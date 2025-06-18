# 🛡️ CIA TRIAD – TryHackMe Professional Report

🔐 Foundation of Cybersecurity.  
✅ **Room:** CIA Triad  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

The *CIA Triad* is the *core model* of information security. It defines the three primary goals every cybersecurity strategy must achieve:  
*Confidentiality*, *Integrity*, and *Availability*. Without these, systems are vulnerable and data becomes worthless.
🧠 This room explains how each component works, why it's important, and how attackers try to break them — and how ethical hackers defend them.
.

---

## 🔺 The CIA Triad Explained

| 🔑 Component     | 🔍 Definition                                        | 🚨 Attacks Threatening It        |
|------------------|-----------------------------------------------------|----------------------------------|
| 🔒 *Confidentiality* | Keeping data private & protected from unauthorized access | Data breach, packet sniffing     |
| 🧬 *Integrity*       | Ensuring data is accurate and unchanged             | Tampering, Man-in-the-Middle     |
| ⚙️ *Availability*    | Ensuring services/data are accessible when needed   | DDoS, ransomware, hardware failure |

---

## 🔐 1. Confidentiality

- 🔍 *Goal:* Only authorized people/systems can view the data.
- 🔐 Techniques: *Encryption*, *Access Control*, *Two-Factor Authentication*
- 🚨 Example Attack:  
  - *Unauthorized access* via password brute force  
  - *Packet sniffing* to read unencrypted data

### ✅ Real-World Example:
Using HTTPS encrypts data in transit to preserve confidentiality.


---

## 🧬 2. Integrity

- 🔍 *Goal:* Protect data from being *modified* or *tampered* with.
- 🔐 Techniques: *Hashing*, *Checksums*, *Digital Signatures*
- 🚨 Example Attack:  
  - *MITM* attack where data is changed before reaching the user

### ✅ Real-World Example:
Software update files are signed with a hash to verify they weren't altered.


---

## ⚙️ 3. Availability

- 🔍 *Goal:* Systems and services are up and running when needed.
- 🔐 Techniques: *Backups*, *Redundancy*, *Firewalls*
*DDoS Protection**
- 🚨 Example Attack:  
  - *DDoS Attack* overwhelms a server  
  - *Ransomware* locks users out

### ✅ Real-World Example:
Banks use backup servers to maintain online banking availability 24/7.


---

## 📚 CIA in Action (Ethical Hacker’s View)

| 🧠 Skill Area        | 💼 Related CIA Element   | 🛠️ Tools or Techniques            |
|----------------------|--------------------------|------------------------------------|
| Penetration Testing  | Confidentiality          | Burp Suite, Nmap, Hydra            |
| Data Validation      | Integrity                | Hash Verification (SHA256)         |
| Network Defense      | Availability             | Fail2Ban, Load Balancers, Firewalls |

---

## ✍️ Author & Branding

### 👨‍💻 Report by:  *🔰 Asibur Khan – Ethical Hacker & Cybersecurity Practitioner**  
GitHub: [Asibur-syber](https://github.com/Asibur-syber)
Crafted with 💡 expertise and 💻 hands-on practice via [TryHackMe.com](https://tryhackme.com)
m)

---

## ✅ File Info

- Save this file as: 03_CIA_Triad_AsiburKhan.md
- Suitable for: GitHub upload 📂, Fiverr portfolio, Client demos

---

## 🧠 Final Words

“If the CIA Triad breaks — security breaks.”  
Understanding and defending **Confidentiality**, **Integrity**, and **Availability** is what makes us true defenders of the digital world.


*This room helped shape my core philosophy in cybersecurity.*
