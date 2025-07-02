# 🧑‍💻 ASIBUR RAHAMAN  
Ethical Hacker | Windows Recon Specialist | Red Team Enthusiast  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🪟 TRYHACKME ROOM REPORT — 08: WINDOWS FUNDAMENTALS 1  
🔗 [Room Link → https://tryhackme.com/room/windowsfundamentals1](https://tryhackme.com/room/windowsfundamentals1)  
📅 *Date Completed:* July 2, 2025  
📂 *Category:* Windows OS Internals  
🎯 *Focus:* File Systems, Control Panel, Task Manager, CMD  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room introduces the key fundamentals of the *Windows operating system*, including file system structures, Control Panel utilities, Task Manager insights, and Command Prompt navigation. Understanding Windows is critical for ethical hackers as it is the most widely used OS in enterprise environments. This knowledge equips learners to explore, enumerate, and manipulate Windows systems through both GUI and CLI.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

### 🔹 1. Windows File System

- Windows primarily uses *NTFS (New Technology File System)*.  
- Important directories under C:\:  
  - C:\Users\ — user profiles and personal data  
  - C:\Program Files\ — installed applications  
  - C:\Windows\ — core operating system files  
- Hidden files and folders can be revealed via *File Explorer → View → Hidden items*.

---

### 🔹 2. Control Panel

- Centralized utility for managing system settings, including:  
  - Network & Internet configurations  
  - User Account management  
  - System & Security options  
- Accessible via *Start → Control Panel* or by running control.exe.

---

### 🔹 3. Task Manager

- Shortcut keys: *Ctrl + Shift + Esc* or *Ctrl + Alt + Del* → Task Manager  
- Displays:  
  - Active processes and applications  
  - Real-time CPU, memory, disk, and network usage  
  - Startup program impact and management  
- Essential for malware detection and system performance troubleshooting.

---

### 🔹 4. Command Prompt (CMD)

- Native Windows CLI tool for system navigation and execution of commands.  
- Common commands:  
  - dir — list directory contents  
  - cd — change directories  
  - tasklist — list running processes  
  - systeminfo — display detailed system information

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command  | Purpose                                              |
|-----------------|------------------------------------------------------|
| dir           | List files in a directory                            |
| cd            | Navigate directories                                 |
| tasklist      | View running tasks/processes                         |
| systeminfo    | Display system hardware and software details        |
| control.exe   | Launch Control Panel                                 |
| Task Manager    | Analyze system processes and resource usage         |

---

## 🖥️ PRACTICAL EXAMPLES

- Navigated to C:\Users\Administrator\Documents using cd in CMD.  
- Executed tasklist to identify currently running processes.  
- Used systeminfo to enumerate Windows OS version and build details.  
- Opened Task Manager to monitor and identify high CPU usage processes.  
- Explored Control Panel's *Programs → Uninstall a Program* for managing software.

---

## 🔐 SECURITY INSIGHTS

| Topic        | Relevance to Pentesting                                |
|--------------|--------------------------------------------------------|
| File System  | Understanding NTFS aids in locating sensitive files and logs. |
| Task Manager | Useful for detecting suspicious or malicious processes. |
| CMD          | Vital for scripting, system enumeration, and persistence. |
| Control Panel| Key for investigating system configurations and security settings. |

---

## 📝 FINAL THOUGHTS

Windows remains the most dominant OS in corporate networks. Proficiency in navigating Windows both through GUI and command line is critical for effective penetration testing. This foundational room prepares learners for deeper Windows exploitation and post-exploitation activities.

---

## 🚀 NEXT STEPS

- Study *Windows Services & Registry* (TryHackMe Room 09)  
- Practice using common Windows enumeration tools like *WinPEAS*  
- Set up a dedicated Windows VM lab for hands-on practice  
- Explore privilege escalation via service misconfigurations and scheduled tasks

---
