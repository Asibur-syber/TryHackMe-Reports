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

### 1. What is Burp Suite Repeater?  
- A Burp module for *manually testing HTTP requests*  
- Enables editing of methods, headers, cookies, body data  
- Excellent for logic bypasses and custom payload testing  

---

### 2. Capturing and Sending Requests to Repeater  
1. Enable *Intercept* from Burp's Proxy tab  
2. Perform action on the web (e.g., login or search)  
3. Request is intercepted → Right-click → *Send to Repeater*  
4. Repeater tab opens with full editable request  

---

### 3. Modifying HTTP Requests  
- Change HTTP method (GET ⇄ POST)  
- Edit headers (User-Agent, Referer)  
- Inject SQLi or XSS payloads in parameters  
- Modify cookies to test role escalation  

---

### 4. Analyzing Server Response  
- Observe response status codes:  
  - 200 OK → Success  
  - 403 Forbidden → Access denied  
  - 500 Internal Error → Crashed due to payload  
- Compare original vs modified responses to find bypasses  

---

### 5. Real Pentesting Scenarios Using Repeater  

| Test Type           | Description                                       |
|---------------------|---------------------------------------------------|
| Brute-force Login   | Manually test multiple password combinations      |
| SQL Injection       | Inject ' OR '1'='1 in login fields              |
| XSS Payload         | Test for script injection in input/output         |
| Cookie Tampering    | Change role=user to role=admin                |
| CSRF Replay         | Resend form POSTs without tokens                  |

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Feature         | Purpose                                         |
|------------------------|-------------------------------------------------|
| Burp Suite Repeater    | Manual request crafting & logic testing         |
| Burp Proxy             | Intercepts HTTP traffic to send to Repeater     |
| Firefox Dev Tools      | Inspect request headers and responses           |
| OWASP Juice Shop       | Practice vulnerable app for Repeater usage      |
| HTTP Headers           | View/Modify User-Agent, Cookies, Host, etc.     |

---

## 🖥️ PRACTICAL EXAMPLES

### ✅ Example 1: Modify Login Request for Brute Force

```http
POST /login HTTP/1.1
Host: vulnerable-site.com
Content-Type: application/x-www-form-urlencoded

username=admin&password=admin123
