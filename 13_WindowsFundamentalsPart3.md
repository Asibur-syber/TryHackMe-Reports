# 🪟 WINDOWS FUNDAMENTALS – PART 3 – TryHackMe Professional Report

🧠 Dive Deeper into Windows OS Internals | 🛡️ Prepare for Real-World Scenarios  
✅ **Room:** Windows Fundamentals Part 3  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/windowsfundamentals3)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

This room completes the *Windows Fundamentals* series, focusing on more *advanced internal tools*, *event logs*, *task scheduler*, and *Windows Defender*. These concepts are vital in detecting intrusions, defending endpoints, and understanding attacker behavior on a Windows system.

---

## 🔑 Key Concepts Covered

| 🔸 Topic               | 🔍 Description                                                    |
|------------------------|------------------------------------------------------------------|
| 📂 File Extensions     | File visibility and hiding techniques in Windows                 |
| 🗓️ Task Scheduler       | Automating tasks – used by both admins and attackers             |
| 📄 Event Logs          | Tracking user actions, logon events, and system changes          |
| 🧱 Windows Defender     | Default antivirus/antimalware for modern Windows environments    |
| 🔍 Autoruns & Startup   | How to find programs that run at boot                           |

---

## 🧪 Lab Activities Overview

| 🛠️ Activity                     | 💻 Description                                        |
|-------------------------------|------------------------------------------------------|
| Enabled hidden file extensions | Protected against malware masking                   |
| Explored Task Scheduler        | Observed scheduled tasks and created a custom task  |
| Checked Event Viewer           | Viewed logs for login attempts and alerts           |
| Tested Defender functionality  | Verified scan status and exclusions list            |
| Explored Autoruns              | Detected startup programs and registry entries      |

---

## 📈 Sample Commands & Actions

```powershell
# Open Event Viewer
eventvwr.msc

# Run Defender Scan
Start-MpScan -ScanType QuickScan

# Check Startup Tasks
taskschd.msc

# View Autorun Programs
msconfig
