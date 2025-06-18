# 🌐 WEB APPLICATION SECURITY – TryHackMe Professional Report

💻 Break the Web to Defend It | 🔐 Learn OWASP, XSS, and More  
✅ **Room:** Web Application Security  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/webapplicationsecurity)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

Web applications are *prime targets* for hackers. This room covers the most common vulnerabilities found in websites — from broken authentication to injection attacks — and teaches how to exploit and protect them.
🎯 Learn to hack web apps so you can defend them better!
!

This report presents hands-on experience with OWASP Top 10 vulnerabilities, web server basics, tools like Burp Suite, and practical exploitation.

---

## 🛡️ Key Vulnerabilities Covered

| 🛠️ Vulnerability       | ⚠️ Description                                | 🔓 Real-World Risk                     |
|------------------------|-----------------------------------------------|----------------------------------------|
| 🔐 Broken Auth         | Poor login systems, session ID leaks          | Account hijacking                      |
| 💉 SQL Injection       | Unsanitized database input                    | Database dump, credential theft        |
| 🔗 IDOR                | Insecure direct object references             | Data leakage between users             |
| 🧼 XSS (Cross-site Scripting) | Injecting scripts in pages              | Cookie theft, defacement               |
| 🧪 CSRF                | Forging authenticated requests                | Unauthorized changes                   |

---

## 🧪 Lab Activities Summary

| 🛠️ Tool Used     | 💻 Purpose                                     |
|------------------|------------------------------------------------|
| *Burp Suite*    | Intercept & manipulate HTTP requests           |
| *Firefox DevTools* | Inspect elements, cookies, JavaScript        |
| *SQLmap*        | Automate SQL Injection testing                 |
| *XSS Hunter*    | Track XSS payloads                             |

---

## 🔍 Sample Web Exploits

### 🩸 SQL Injection (Manual)
```bash
# URL Parameter Injection
http://example.com/page.php?id=1' OR '1'='1
