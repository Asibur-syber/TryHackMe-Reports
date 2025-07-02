# 🧑💻 ASIBUR RAHAMAN  
*Ethical Hacker | Windows Recon Specialist | Red Team Enthusiast*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🪟 TRYHACKME ROOM REPORT — 09: WINDOWS FUNDAMENTALS 2  
🔗 [Room Link → https://tryhackme.com/room/windowsfundamentals2](https://tryhackme.com/room/windowsfundamentals2)  
📅 **Date Completed:** July 2, 2025  
📂 **Category:** Windows OS Internals  
🎯 **Focus:** Registry, User Accounts, Permissions, Services, UAC  
🧩 **Difficulty:** 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room delves deeper into the internal workings of the **Windows operating system**, focusing on key areas that are often targeted or manipulated by attackers: the **Windows Registry**, **User Accounts**, **Permissions**, **Background Services**, and **User Account Control (UAC)**. Understanding these components is vital for ethical hackers to identify misconfigurations, persist on systems, or elevate privileges in Windows environments.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 🔹 1. Windows Registry

- The Windows Registry is a hierarchical database storing low-level settings for Windows OS and applications.
- Launched via: `regedit`
- Five root keys include:
  - `HKEY_CLASSES_ROOT`
  - `HKEY_CURRENT_USER`
  - `HKEY_LOCAL_MACHINE` ✅ (most important)
  - `HKEY_USERS`
  - `HKEY_CURRENT_CONFIG`

📌 *Sensitive configurations, autorun entries, and malware persistence are often stored here.*

---

### 🔹 2. User Accounts & SIDs

- View user accounts: `net user`
- Each user has a **SID (Security Identifier)** that uniquely identifies them.
- The `Administrator` account is often disabled by default.

📌 *Account enumeration is essential for privilege escalation and post-exploitation.*

---

### 🔹 3. File & Folder Permissions

- Windows applies **Access Control Lists (ACLs)** to define what users can do with files/folders.
- Permissions include: **Read, Write, Modify, Full Control**
- GUI path: Right-click → Properties → Security Tab

📌 *Misconfigured permissions can lead to sensitive data exposure or code execution.*

---

### 🔹 4. Services (Background Processes)

- Services are long-running system processes.
- Managed via: `services.msc` or CLI (`sc query`)
- Important service configuration can be viewed using: `sc qc <service-name>`

📌 *Services running as SYSTEM or with weak configs are common privilege escalation targets.*

---

### 🔹 5. User Account Control (UAC)

- UAC prompts users when administrative privileges are required.
- UAC settings can be modified via:  
  Control Panel → User Accounts → Change UAC Settings

📌 *UAC bypass is a known tactic used by attackers to silently elevate privileges.*

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command      | Purpose                                                  |
|---------------------|----------------------------------------------------------|
| `regedit`           | Open Windows Registry Editor                             |
| `net user`          | List all user accounts                                   |
| `icacls <path>`     | View folder/file permission details                      |
| `whoami /groups`    | Show current user’s group membership and privileges      |
| `sc query`          | List all services running on the system                  |
| `sc qc <service>`   | Display configuration details of a specific service      |
| `services.msc`      | GUI-based Service Manager                                |

---

## 🖥️ PRACTICAL EXAMPLES

- 🧪 Launched **Registry Editor**: `regedit` → browsed to `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services`
- 🧪 Listed user accounts: `net user`  
- 🧪 Checked Administrator account status: `net user Administrator`
- 🧪 Explored file permissions with: `icacls C:\Users`
- 🧪 Opened Services manager: `services.msc`  
- 🧪 Viewed UAC level in Control Panel → UAC Settings  
- 🧪 Inspected a service config: `sc qc wuauserv`

---

## 🔐 SECURITY INSIGHTS

| Topic          | Security Relevance                                           |
|----------------|--------------------------------------------------------------|
| Registry       | Used for persistence, malware configs, and system tweaks     |
| User Accounts  | Identifying admin accounts is critical for lateral movement  |
| Permissions    | Weak ACLs enable privilege escalation or data exfiltration    |
| Services       | Poorly configured services can lead to SYSTEM-level access   |
| UAC            | Attackers often try to bypass UAC prompts for silent escalation |

---

## 📝 FINAL THOUGHTS

Understanding the internal mechanics of Windows is non-negotiable for any serious penetration tester. This room empowers learners to confidently inspect user accounts, navigate the registry, audit permissions, and analyze services — all of which are essential for enumeration, privilege escalation, and post-exploitation in real-world Windows environments.

---

## 🚀 NEXT STEPS

- Start **Room 10: Windows Fundamentals 3** to continue with Windows OS mastery  
- Explore **WinPEAS** for automated Windows enumeration  
- Try a real-world vulnerable box like “Blue” or “Bounty Hacker”  
- Create a **GitHub walkthrough** for this room with screenshots  
- Add a “Windows Recon” Fiverr gig offering this type of report

---
