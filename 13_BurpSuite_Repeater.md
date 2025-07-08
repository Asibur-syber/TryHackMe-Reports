# 🧑‍💻 ASIBUR RAHAMAN  
Ethical Hacker | Web Recon Specialist | Burp Suite Explorer  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🧪 TRYHACKME ROOM REPORT — 13: BURP SUITE REPEATER  
🔗 [Room Link → https://tryhackme.com/room/burpsuiterepeater](https://tryhackme.com/room/burpsuiterepeater)  
📅 Date Completed: July 8, 2025  
📂 Category: Manual Web Application Testing  
🎯 Focus: HTTP Request Manipulation, Repeater, Web Logic Testing  
🧩 Difficulty: 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room focuses on one of the most powerful features of Burp Suite — the *Repeater* tab. It allows ethical hackers to *manually resend and modify HTTP requests* and analyze how a server reacts.

This is essential for discovering vulnerabilities such as:

- SQL Injection (SQLi)  
- Cross-Site Scripting (XSS)  
- CSRF (Cross-Site Request Forgery)  
- Logic flaws in authentication & session handling  

Repeater gives you *full control* over each request, making it a vital tool for professional penetration testers and bug bounty hunters.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

### 1. 🔎 What is Burp Suite Repeater?  
- A Burp module for *manually testing HTTP requests*  
- Enables editing of methods, headers, cookies, body data  
- Excellent for logic bypasses and custom payload testing  

---

### 2. 🎣 Capturing and Sending Requests to Repeater  
1. Enable *Intercept* from Burp's Proxy tab  
2. Perform any action (e.g., login, search)  
3. Request gets intercepted  
4. Right-click → *Send to Repeater*  
5. Repeater tab opens the request for editing

---

### 3. 🧪 Modifying HTTP Requests  
- Change HTTP method (GET ⇄ POST)  
- Modify headers (User-Agent, Referer)  
- Inject payloads (SQLi, XSS) in input fields  
- Tamper with cookies for *role escalation* or session hijacking  

---

### 4. 🧵 Analyzing Server Response  
- Check *HTTP status codes* and *response messages*  
  - 200 OK → Request successful  
  - 302 Found → Redirected (possibly successful login)  
  - 403 Forbidden → Access denied  
  - 500 Internal Server Error → Possible crash due to payload  
- Compare original and modified responses to identify weaknesses

---

### 5. 🛠️ Real Pentesting Scenarios Using Repeater  

| Test Type           | Description                                       |
|---------------------|---------------------------------------------------|
| Brute-force Login   | Manually test multiple passwords                  |
| SQL Injection       | Inject ' OR '1'='1 in login fields              |
| XSS Payload         | Inject <script>alert(1)</script> in inputs      |
| Cookie Tampering    | Change role=user → role=admin                 |
| CSRF Replay         | Resend POST requests without CSRF tokens          |

---

## 🧰 TOOLS & TECHNIQUES USED

| Tool / Feature         | Purpose                                         |
|------------------------|-------------------------------------------------|
| **Burp Suite Repeater**| Modify, resend, and analyze HTTP requests       |
| *Burp Proxy*         | Capture live browser traffic                    |
| *Manual Payloads*    | For XSS, SQLi, CSRF testing                     |
| **HTTP Header Editing**| Tamper with User-Agent, Referer, Cookies        |

---

## 🖥️ PRACTICAL EXAMPLES

### ✅ Example 1: Modify Login Request for Brute Force

```http
POST /login HTTP/1.1
Host: vulnerable-site.com
Content-Type: application/x-www-form-urlencoded

username=admin&password=admin123

➡️ In Repeater, change password value and observe response:

username=admin&password=123456
username=admin&password=letmein
username=admin&password=password

Status Code 200 or 302 = Successful Login

Status Code 403 or 401 = Blocked or Failed



---

### ✅ Example 2: SQL Injection Payload

POST /login HTTP/1.1
Host: vulnerable-site.com
Content-Type: application/x-www-form-urlencoded

username=admin' OR '1'='1&password=dummy

➡️ If it bypasses login → Target is vulnerable to SQLi


---

### ✅ Example 3: Cookie Tampering for Privilege Escalation

Cookie: sessionid=abc123; role=user

➡️ Modify in Repeater:

Cookie: sessionid=abc123; role=admin

➡️ If admin panel opens → Privilege escalation exists


---

🔐 SECURITY INSIGHTS

Feature	Potential Risk/Abuse

Request Editing	Bypass auth or input filters
SQLi Payloads	Database dumping or authentication bypass
Cookie Manipulation	Role escalation, session hijacking
CSRF Replay	Force unauthorized actions using forged POST
Method Switching	PUT or DELETE could allow data tampering



---

📝 FINAL THOUGHTS

Burp Suite Repeater is one of the most effective tools for real-world testing. It gives the power to manually craft, resend, and analyze HTTP requests — which is essential for catching flaws that automation often misses.

Knowing how to use Repeater is a core skill for every web pentester.


---

🚀 NEXT STEPS

Document this room as part of your GitHub pentest portfolio

Practice real Repeater testing in vulnerable apps like Juice Shop

Combine Repeater with Intruder for automation

Move to Room 14: Burp Suite Intruder to learn semi-automated payload delivery


---
