# 🧑‍💻 ASIBUR RAHAMAN  
Ethical Hacker | Web Recon Specialist | Burp Suite Explorer  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🌐 TRYHACKME ROOM REPORT — 12: HOW WEBSITES WORK  
🔗 [Room Link → https://tryhackme.com/room/howwebsiteswork](https://tryhackme.com/room/howwebsiteswork)  
📅 Date Completed: July 5, 2025  
📂 Category: Web Fundamentals & HTTP Concepts  
🎯 Focus: DNS, HTTP Requests, Responses, Cookies, Authentication  
🧩 Difficulty: 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room provides a beginner-friendly but crucial foundation for understanding how websites operate. It explores the full web request–response cycle, DNS resolution, static vs dynamic content, cookies, sessions, authentication, and real-world examples of web traffic.

This knowledge is *mandatory* before attempting Burp Suite, XSS, SQL Injection, or API hacking. Without mastering these web basics, ethical hacking skills remain incomplete.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

### 1. DNS Resolution  
- Translates domain (e.g., facebook.com) into IP address  
- Example: facebook.com → 157.240.20.35  
- DNS spoofing can lead to phishing or redirection attacks  

### 2. HTTP/HTTPS Request  
- GET / POST methods used to request/submit data  
- Headers like Host, User-Agent, Cookie included  
- Sent from browser to web server  

### 3. HTTP Response  
- Server sends HTML, CSS, JS in response  
- Example response status: 200 OK  
- Browser renders the response into a visual page  

### 4. Static vs Dynamic Websites  
- Static: Only HTML/CSS (read-only)  
- Dynamic: Includes PHP, JS, Python with DB interaction  
- Dynamic sites are vulnerable to SQLi, XSS, and auth bypass  

### 5. HTTP Methods  
| Method | Purpose           | Example                   |
|--------|-------------------|---------------------------|
| GET    | Retrieve data     | GET /profile?id=5         |
| POST   | Submit data       | POST /login               |
| PUT    | Create/replace    | PUT /api/users            |
| DELETE | Remove resource   | DELETE /api/delete?id=2   |

### 6. Cookies  
- Sent by server to browser to store session data  
- Example: Set-Cookie: sessionid=abc123; Secure; HttpOnly  
- Secure flag: only over HTTPS  
- HttpOnly: not accessible by JS (protects from XSS)

### 7. Authentication Flow  
1. User submits login form (POST request)  
2. Server verifies credentials  
3. Generates session token  
4. Sends cookie back to browser  
5. Browser stores it → used for future requests  

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command      | Purpose                                          |
|---------------------|--------------------------------------------------|
| Burp Suite          | Intercept, modify HTTP requests/responses       |
| Firefox Dev Tools   | Inspect HTML, cookies, headers                  |
| Wireshark           | Analyze raw network packets (HTTP/HTTPS)        |
| cURL                | Test HTTP methods via CLI                       |
| Postman             | Interact with and test REST APIs                |

---

## 🖥️ PRACTICAL EXAMPLES

- Used Burp Suite to intercept a login form submission  
- Observed GET and POST requests and response status codes  
- Detected cookie creation in server response  
- Used Dev Tools to explore cookies and local storage  
- Performed simple Brute Force demo via Burp Intruder  

---

## 🔐 SECURITY INSIGHTS

| Web Feature     | Potential Exploit or Weakness                  |
|------------------|------------------------------------------------|
| DNS              | DNS Spoofing → redirect to malicious IPs      |
| HTTP Methods     | Improper POST/PUT access → Data modification  |
| Cookies          | If insecure, leads to session hijacking       |
| Authentication   | Weak passwords → Brute Force risk             |
| Dynamic Content  | SQL Injection, XSS injection risks            |

---

## 📝 FINAL THOUGHTS

A strong understanding of *web mechanics* is essential for any cybersecurity professional. Knowing how the web communicates behind the scenes empowers hackers to properly exploit, secure, and test applications.

This room forms the root of learning for Burp Suite, XSS, API attacks, Cookie hijacking, and more.

---

## 🚀 NEXT STEPS

- Upload this markdown report to GitHub for your portfolio  
- Practice GET/POST interception using Burp Suite  
- Explore cookies and headers using Firefox Dev Tools  
- Begin *Room 13: Burp Suite Repeater* to learn web request replaying  
- Convert this report to PDF for Fiverr showcase  
- Prepare a client-ready pentest walkthrough involving web forms  

---
