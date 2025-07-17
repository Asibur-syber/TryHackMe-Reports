# 🧑‍💻 ASIBUR RAHAMAN  
**Ethical Hacker | Web Recon Specialist | Brute Force Analyst**  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🔓 TRYHACKME ROOM REPORT — 17: BRUTE FORCE  
🔗 [Room Link → https://tryhackme.com/room/bruteforce](https://tryhackme.com/room/bruteforce)  
📅 *Date Completed:* July 12, 2025  
📂 *Category:* Web Application Security  
🎯 *Focus:* Password Cracking, Dictionary Attacks, Login Bypass  
🧩 *Difficulty:* 🟡 Beginner to Intermediate

---

## 🧠 EXECUTIVE SUMMARY

The **Brute Force** room demonstrates how attackers systematically guess usernames and passwords to gain unauthorized access. This is one of the most **commonly used attack vectors** in real-world scenarios and is highly relevant in **penetration testing**.

This room covers:

- Dictionary-based brute force attacks  
- Username enumeration techniques  
- Hydra for automated brute force  
- Web form and SSH-based login brute forcing  

---

## 🎯 STEP-BY-STEP LEARNING BREAKDOWN

| Step | Focus Area                 | Description |
|------|----------------------------|-------------|
| 1️⃣ | **What is Brute Force?**    | Overview of attack types |
| 2️⃣ | **Hydra Tool Basics**       | Command-line tool for brute forcing |
| 3️⃣ | **Web Login Brute Force**   | Using Hydra against a login form |
| 4️⃣ | **SSH Login Brute Force**   | Attacking SSH using known username list |
| 5️⃣ | **User Enumeration**        | Discovering valid usernames |
| 6️⃣ | **Mitigation Techniques**   | Protecting against brute force

---

## 🧰 TOOLS, COMMANDS & PAYLOADS

| Tool / Command | Usage |
|----------------|-------|
| `hydra -l <user> -P <wordlist> <ip> ssh` | SSH brute force |
| `hydra -L <users.txt> -P <passwords.txt> <ip> http-post-form "<path>:<payload>:F=Incorrect"` | Web login |
| `wfuzz`, `dirb` | Directory brute forcing |
| `rockyou.txt` | Common password wordlist |
| `cewl`, `crunch` | Wordlist generation |
| `Burp Suite` | Capture login POST request |

---

## 🧪 PRACTICAL EXAMPLES (LAB CASES)

✅ **Hydra SSH Brute Force**  
- **Command**:  
  `hydra -l admin -P /usr/share/wordlists/rockyou.txt ssh://<THM_IP>`  
- **Result**: Found password → `admin:password123`

✅ **Web Login Brute Force (POST)**  
- **Command**:  
  `hydra -L users.txt -P passwords.txt <THM_IP> http-post-form "/login:username=^USER^&password=^PASS^:Invalid password"`  
- **Result**: Successful login found

✅ **Username Enumeration**  
- Try usernames manually on login page  
- Observe responses (e.g., `User not found`, `Wrong password`)  

---

## 🔍 RESPONSE ANALYSIS STRATEGY

| Symptom                       | Interpretation |
|-------------------------------|----------------|
| 🟠 “User not found” error      | Try other usernames |
| 🔴 “Invalid password” message  | Valid username, wrong password |
| ✅ “Welcome” or redirect       | Login successful |
| 🐌 Slow response               | Possible rate limiting or lockout |

---

## 🔐 SECURITY INSIGHTS & ATTACK PATHS

| Attack Vector | Risk | Mitigation |
|---------------|------|------------|
| Brute Force via Login Form | Credential stuffing | Rate limiting, CAPTCHA |
| SSH Password Guessing | Remote shell access | Disable password login, use keys |
| Enumeration via error message | Username discovery | Standardized error messages |

---

## 🖼️ RECOMMENDED SCREENSHOTS (GitHub/Fiverr)

- ✅ Hydra terminal output with credentials found  
- ✅ Burp Suite POST request analysis  
- ✅ Web login page (before & after login)  
- ✅ Error messages (for enum detection)  
- ✅ `rockyou.txt` usage example in command

---

## 📝 FINAL THOUGHTS

This room gives a hands-on intro to brute force attacks and how they work on both **web and SSH interfaces**. Mastering these techniques is crucial before diving into **real CTFs or client-side pen-testing gigs**.

- Understand **login mechanics**  
- Observe **error messages & patterns**  
- Always test with **legal consent**  

---

## 🚀 NEXT STEPS (ASIBUR RAHAMAN ACTION PLAN)

- ✅ Add screenshots from Hydra + Burp  
- ✅ Upload this report to GitHub under `TryHackMe-Reports`  
- ✅ Create Fiverr Gig: “I will test your website for login brute force flaws”  
- ▶️ Start Next Room: **Broken Authentication (Room 18)**

---

## 📁 FILE NAME FOR GITHUB

```bash
17_BRUTE_FORCE_Asibur.md
