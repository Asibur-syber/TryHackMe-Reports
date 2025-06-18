# 🪟 WINDOWS FUNDAMENTALS – PART 2 – TryHackMe Professional Report

🧠 Master the Basics of Windows OS | 🔍 Learn Key Concepts for Pentesting  
✅ **Room:** Windows Fundamentals Part 2  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/windowsfundamentals2)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

This room dives into fundamental Windows operating system concepts crucial for cybersecurity professionals, such as user account enumeration, permission management, and service handling. Understanding these basics helps in identifying potential vulnerabilities and attack vectors in Windows environments.

---

## 🔑 Key Concepts Covered

| 🔸 Topic              | 🔍 Description                                                       |
|----------------------|---------------------------------------------------------------------|
| 👤 User Enumeration   | Listing local users and groups using net user and net localgroup |
| 🔐 Permissions        | Checking file and folder access rights using icacls               |
| ⚙️ Windows Services    | Managing services via sc and PowerShell                           |

---

## 🧪 Lab Activities Overview

| 🛠️ Activity                  | 💻 Description                                   |
|-----------------------------|-------------------------------------------------|
| net user                  | Enumerated user accounts                         |
| net localgroup            | Checked group memberships                        |
| icacls                   | Reviewed file and folder permissions             |
| sc query                 | Listed running Windows services                   |
| PowerShell Get-Service   | Gathered service details and status               |

---

## 📈 Sample Commands & Outputs

```powershell
# List users
net user

# Check administrators group members
net localgroup administrators

# View permissions of a folder
icacls C:\Users\Public

# Query Windows services
sc query

# PowerShell service listing
Get-Service | Where-Object {$_.Status -eq 'Running'}
