# 🛡️ TryHackMe Report: Burp Suite Basics

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [Burp Suite Basics on TryHackMe](https://tryhackme.com/room/burpsuitebasics)

---

## 🧠 1. Room Overview

This room introduces *Burp Suite*, a powerful web vulnerability scanner and proxy tool used widely in penetration testing.  
It covers the basics of intercepting, modifying, and replaying HTTP requests to find security flaws in web applications.

---

## 🛠️ 2. Tools Used

| Tool       | Purpose                          |
|------------|---------------------------------|
| Burp Suite | Intercept and modify HTTP traffic|
| Browser    | Sending and receiving requests   |
| Terminal   | Running proxy and tools          |

---

## 🚀 3. Step-by-Step Learning & Exploitation

### Step 1: Setting up Burp Proxy
- Configured Burp Suite as a proxy to intercept browser traffic.
- Installed Burp CA certificate in browser to avoid SSL issues.

### Step 2: Intercepting Requests
- Captured HTTP requests between browser and target web app.
- Modified parameters to test for input validation vulnerabilities.

### Step 3: Using Repeater & Intruder
- Sent requests to *Repeater* to manually test different payloads.
- Used *Intruder* to automate fuzzing and brute force attack simulations.

### Step 4: Analyzing Responses
- Examined HTTP responses for error messages, data leakage, and behavioral changes.
- Logged findings for further exploitation and reporting.

---

## 🎯 4. Captured Flags

- ✅ User Flag: THM{Burp_Suite_Basics_Mastered}

---

## 📚 5. Key Takeaways

- Learned how to configure and use Burp Suite proxy effectively.
- Practiced manual testing of web inputs and automation tools inside Burp.
- Gained understanding of HTTP request-response lifecycle in pen testing.
- Recognized the importance of modifying requests to find hidden vulnerabilities.

---

## 📸 6. Supporting Screenshots
📌 **Burp Proxy Intercepting a Request**  
 
![burp-proxy](burp_proxy.png)
📌 **Using Repeater to Test Payloads**  
 
![burp-repeater](burp_repeater.png)


---

## ✍️ 7. Personal Notes

- Burp Suite is essential for web app pentesters; mastering basics boosts testing efficiency.
- Always keep your proxy configuration secure and updated.
- Practice with different web apps to understand varied behaviors.

---

🔚 *End of Report*  
📁 GitHub Repository: [TryHackMe-Reports](https://github.com/Asibur-syber/TryHackMe-Reports)
