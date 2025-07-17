# 🧑‍💻 ASIBUR RAHAMAN  
**Ethical Hacker | Web Recon Specialist | Authentication Tester**  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🔐 TRYHACKME ROOM REPORT — 18: BROKEN AUTHENTICATION  
🔗 [Room Link → https://tryhackme.com/room/brokenauthentication](https://tryhackme.com/room/brokenauthentication)  
📅 *Date Completed:* July 13, 2025  
📂 *Category:* Web Application Security (OWASP Top 10)  
🎯 *Focus:* Broken Login Logic, Session Hijacking, Credential Stuffing  
🧩 *Difficulty:* 🟡 Beginner to Intermediate

---

## 🧠 EXECUTIVE SUMMARY

The **Broken Authentication** room demonstrates how web applications can fail to properly handle user authentication — allowing attackers to:

- **Bypass login pages**
- **Hijack user sessions**
- **Exploit poor password practices**
- **Enumerate users or reuse passwords**

These vulnerabilities fall under the **OWASP Top 10** and are **frequently found** in real-world bug bounty programs and penetration testing scopes.

---

## 🎯 STEP-BY-STEP LEARNING BREAKDOWN

| Step | Topic                     | Description |
|------|---------------------------|-------------|
| 1️⃣ | **Understanding Auth Flow** | Basic login workflow and its weak points |
| 2️⃣ | **Brute Force Login**       | Exploiting weak passwords |
| 3️⃣ | **Credential Stuffing**     | Using leaked passwords from data breaches |
| 4️⃣ | **Session Hijacking**       | Stealing cookies to access user accounts |
| 5️⃣ | **Insecure Redirects**      | Exploiting weak session control or redirects |

---

## 🧰 TOOLS, COMMANDS & PAYLOADS

| Tool / Payload       | Purpose |
|----------------------|---------|
| `hydra`, `wfuzz`     | Login brute force |
| `Burp Suite`         | Intercept login & hijack cookies |
| `rockyou.txt`        | Common password list |
| `Developer Tools`    | View session cookies |
| `whatweb`, `dirb`    | Recon and endpoint discovery |

---

## 🧪 PRACTICAL EXAMPLES (LAB CASES)

✅ **Brute Forcing Login Page**  
- **Command**:  
  `hydra -l admin -P rockyou.txt <THM_IP> http-post-form "/login:username=^USER^&password=^PASS^:Invalid password"`  
- **Result**: Found correct password → Logged in as `admin`

✅ **Session Hijacking**  
- **Method**:  
  - Capture session cookie after login  
  - Replay session in another browser  
- **Result**: Full access without login

✅ **Credential Stuffing**  
- **Approach**: Use known email + password combo from breach list  
- **Result**: Bypassed login with reused credential

✅ **Error-Based Enumeration**  
- **Test**: Enter wrong usernames  
- **Response**: `User does not exist`  
- **Result**: User enumeration possible

---

## 🔍 RESPONSE ANALYSIS STRATEGY

| Observation                     | Interpretation |
|----------------------------------|----------------|
| ❌ “User not found” error         | Valid for enumeration |
| 🔴 “Invalid password” only        | Valid username, try more passwords |
| ✅ Cookie stays same after logout | Poor session management |
| 🧪 Cookie works across sessions   | Vulnerable to hijacking |

---

## 🔐 SECURITY INSIGHTS & ATTACK PATHS

| Attack Vector         | Risk                        | Mitigation |
|------------------------|-----------------------------|------------|
| Weak password logic    | Account takeover             | Enforce strong passwords |
| No lockout mechanism   | Brute force possible         | Rate-limiting, CAPTCHA |
| Reusable session cookie| Account hijack               | Invalidate session on logout |
| Informative error msgs | Username enumeration         | Use generic errors |

---

## 🖼️ RECOMMENDED SCREENSHOTS (For GitHub/Fiverr)

- ✅ Hydra output with cracked credentials  
- ✅ Burp Suite intercept of login POST request  
- ✅ Session cookie view in DevTools  
- ✅ Replay of stolen cookie access  
- ✅ Screenshot of error messages for bad login

---

## 📝 FINAL THOUGHTS

Broken Authentication is one of the **most dangerous web flaws** — it can fully compromise user data and control. This room teaches us the importance of:

- Validating authentication logic  
- Securing session tokens  
- Using multi-factor authentication (MFA)  
- Avoiding reuse of credentials

This knowledge directly helps in **bug bounty**, **client pentests**, and **secure development**.

---

## 🚀 NEXT STEPS (ASIBUR RAHAMAN ACTION PLAN)

- ✅ Upload this report to GitHub  
- 📷 Add screenshots of session hijack test  
- 🛠️ Launch Fiverr Gig: “I will test your site for authentication bypass”  
- ▶️ Start Next Room: **OWASP TOP 10 (Room 19)**

---

## 📁 FILE NAME FOR GITHUB

```bash
18_BROKEN_AUTHENTICATION_Asibur.md
