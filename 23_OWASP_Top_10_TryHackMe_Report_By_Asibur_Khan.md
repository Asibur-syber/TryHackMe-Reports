# 🛡️ TryHackMe Report: OWASP Top 10

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [OWASP Top 10 on TryHackMe](https://tryhackme.com/room/owasptop10)

---

## 🧠 1. Room Overview

This room dives deep into the *OWASP Top 10 vulnerabilities* — the most critical security risks to web applications.  
Understanding these vulnerabilities is essential for any security professional aiming to protect or audit web apps effectively.

---

## 🛠️ 2. Tools & Techniques Used

| Tool           | Purpose                                |
|----------------|----------------------------------------|
| Burp Suite     | Web app vulnerability scanning         |
| OWASP ZAP      | Automated vulnerability assessment     |
| Nikto          | Web server scanning and misconfig checks |
| Manual Testing | Input validation, authentication tests |

---

## 🚨 3. Summary of OWASP Top 10 Vulnerabilities

| Vulnerability                | Description                                   | Example / Mitigation                    |
|-----------------------------|-----------------------------------------------|---------------------------------------|
| *A1: Injection*           | SQL, OS, LDAP injection flaws                  | Use prepared statements, input validation |
| *A2: Broken Authentication* | Weak auth allowing account compromise         | Implement MFA, secure password policies   |
| *A3: Sensitive Data Exposure* | Poor encryption or data leaks                 | Use strong encryption, HTTPS              |
| *A4: XML External Entities (XXE)* | XML parser vulnerabilities                  | Disable external entity processing        |
| *A5: Broken Access Control* | Unauthorized access due to improper controls  | Enforce role-based access, audit logs     |
| *A6: Security Misconfiguration* | Default configs, open cloud storage          | Harden servers, remove unused features    |
| *A7: Cross-Site Scripting (XSS)* | Injecting malicious scripts into web pages  | Use output encoding, Content Security Policy |
| *A8: Insecure Deserialization* | Deserialization flaws enabling attacks      | Avoid unserializing untrusted data         |
| *A9: Using Components with Known Vulnerabilities* | Using outdated libraries or components   | Regularly update dependencies              |
| *A10: Insufficient Logging & Monitoring* | Lack of audit and alerting systems        | Implement real-time monitoring and alerts |

---

## 🧪 4. Approach & Exploitation Steps

### Step 1: Recon & Scanning
- Used *Burp Suite* proxy to intercept requests and test for injection points.
- Ran *Nikto* to identify web server misconfigurations and outdated software.

### Step 2: Testing Authentication
- Manually tested login forms for weak credentials and session management flaws.
- Checked for password reset and MFA bypass possibilities.

### Step 3: Exploiting XSS & Injection
- Injected payloads in input fields to confirm reflected and stored XSS.
- Tested SQL injection via URL parameters using Burp Intruder.

### Step 4: Review of Access Control
- Attempted to access admin functions as a normal user.
- Verified role-based access controls and forced browsing protections.

---

## 🎯 5. Captured Flags

- ✅ User Flag: THM{OWASP_Top_10_Success}

---

## 📘 6. Key Learnings

- 🔥 Deep understanding of each OWASP Top 10 risk with practical testing methods.
- 🛠️ Gained hands-on experience with Burp Suite and Nikto tools.
- 💡 Learned how to identify and exploit common vulnerabilities step-by-step.
- 📝 Importance of comprehensive testing beyond automated scanners.

---

## 📸 7. Supporting Screenshots
📌 **Burp Suite Intercepting Injection Payload**  
 
![burp-inject](burp_injection.png)
📌 **Nikto Scan Result Highlighting Vulnerabilities**  
 
![nikto-scan](nikto_scan.png)


---

## ✍️ 8. Personal Notes

- OWASP Top 10 is a must-know foundation for every web app pentester.
- Manual verification complements automated tools to catch edge cases.
- Continuous learning is necessary as web technologies evolve rapidly.

---

🔚 *End of Report*  
📁 GitHub Repository: [TryHackMe-Reports](https://github.com/Asibur-syber/TryHackMe-Reports)
