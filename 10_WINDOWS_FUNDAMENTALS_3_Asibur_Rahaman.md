# 🧑‍💻 ASIBUR RAHAMAN  
Ethical Hacker | Windows Recon Specialist | Red Team Enthusiast  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🛡️ TRYHACKME ROOM REPORT — 10: WINDOWS FUNDAMENTALS 3  
🔗 [Room Link → https://tryhackme.com/room/windowsfundamentals3](https://tryhackme.com/room/windowsfundamentals3)  
📅 *Date Completed:* July 3, 2025  
📂 *Category:* Windows Security & Access Control  
🎯 *Focus:* UAC, NTFS Permissions, Firewall, Defender, Group Policy, BitLocker  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

Room 10 focuses on Windows built-in security features: User Account Control (UAC), NTFS permissions, Windows Defender, Windows Firewall, Group Policy, and BitLocker drive encryption. These features are crucial to understand for ethical hacking and penetration testing, as they provide defense layers that attackers attempt to bypass or manipulate.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

### 1. User Account Control (UAC)  
- Prevents unauthorized system changes  
- Prompts for admin approval when elevated rights are needed  
- Runs secure desktop for elevation prompts  

### 2. NTFS Permissions  
- Granular file/folder access control  
- Permissions include Full Control, Modify, Read, Write, and Deny  
- Inheritance controls permission propagation  

### 3. Windows Defender  
- Real-time anti-malware protection  
- Can be managed via GUI or PowerShell  
- Tamper protection prevents unauthorized disabling  

### 4. Windows Firewall  
- Controls inbound/outbound network traffic  
- Custom rules can block or allow applications or ports  
- GUI (wf.msc) allows advanced configuration  

### 5. Group Policy Editor  
- Enforces system-wide security policies  
- Can block apps, restrict access, and configure settings  
- Accessible via gpedit.msc  

### 6. BitLocker  
- Full disk encryption technology  
- Protects data-at-rest from offline attacks  
- Supports TPM, password, and recovery key options  

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command       | Purpose                                      |
|----------------------|----------------------------------------------|
| Start-MpScan       | Run Windows Defender quick scan              |
| gpedit.msc         | Open Group Policy Editor                      |
| wf.msc             | Windows Firewall management                   |
| BitLocker GUI        | Manage drive encryption                       |
| NTFS Permissions GUI | File/folder access control                    |
| UAC Prompt (GUI)     | Admin elevation requests                      |

---

## 🖥️ PRACTICAL EXAMPLES

- Enabled BitLocker on a secondary drive and saved the recovery key  
- Blocked cmd.exe execution for standard users via Group Policy  
- Created outbound firewall rule blocking notepad.exe  
- Used PowerShell to trigger Defender quick scan  
- Modified NTFS permissions to deny write access for Guests on C:\Reports

---

## 🔐 SECURITY INSIGHTS

| Security Feature | Importance in Pentesting                      |
|------------------|----------------------------------------------|
| UAC              | Barrier against silent privilege escalation  |
| NTFS Permissions | Weaknesses lead to data exposure or escalation |
| Defender         | Detects and blocks malware, important to evade |
| Firewall         | Controls network flows, critical for C2 channels |
| Group Policy     | Key for enterprise hardening or attack surface |
| BitLocker        | Protects offline data, requires bypass methods |

---

## 📝 FINAL THOUGHTS

Understanding and mastering these Windows security features provides a solid foundation for real-world penetration testing. Effective enumeration and exploitation often depend on recognizing how these controls function and how they might be bypassed or leveraged.

---

 ## 🚀 NEXT STEPS

- Upload this report to your GitHub portfolio  
- Create screenshots demonstrating key Windows security features  
- Start *Room 11: What is the Web* to begin Web Hacking fundamentals  
- Prepare detailed report for Room 11 in the same professional style  
- Convert reports to PDF for Fiverr and client submissions  
- Begin offering gigs related to Windows security and soon Web penetration testing  
- Familiarize yourself with basic HTTP/HTTPS and web technologies 

---

## 📁 FILE NAME SUGGESTION

```text
10_WINDOWS_FUNDAMENTALS_3_Asibur_Rahaman.md
