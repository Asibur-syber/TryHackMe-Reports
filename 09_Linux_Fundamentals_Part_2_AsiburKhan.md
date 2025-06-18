# 🐧 LINUX FUNDAMENTALS – PART 2 – TryHackMe Professional Report

🧠 Learn. 🔍 Practice. 💻 Hack.  
✅ **Room:** Linux Fundamentals Part 2  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

This room continues our deep dive into *Linux essentials* for aspiring ethical hackers. You'll master *file permissions, ownership, user groups, chmod/chown commands*, and permission escalation—critical concepts every penetration tester must know.
🎯 **Goal:** Understand Linux's permission system to prepare for privilege escalation techniques.
.

---

## 📚 Topics Covered

| 🔸 Topic                | 🔍 Description                                          |
|------------------------|---------------------------------------------------------|
| 📂 File Permissions     | Read, write, execute rights for users, groups, others  |
| 🧑 User Ownership        | Each file has an owner (user) and group                |
| 🧮 chmod Command         | Change permission using symbolic or octal mode         |
| 🧾 chown Command         | Change ownership of files/folders                      |
| 👥 User & Group Mgmt     | Creating, modifying, managing users and groups         |
| 🔐 SUID & Privilege Esc | Concept of privilege escalation using misconfigs       |

---

## 🛠️ Hands-On Tools & Commands

### 📁 View File Permissions

```bash
ls -l              # Detailed list showing permissions
ls -lah /etc       # Hidden + detailed list in /etc

```bash
chmod +x script.sh          # Add execute permission
chmod 755 myfile            # rwxr-xr-x
chmod u+x hello.sh          # Give owner execute permission

```bash
chown root:root myfile      # Change owner and group to root
chown asibur myscript.sh    # Make ‘asibur’ the owner

```bash
adduser hacker101           # Create a new user
passwd hacker101            # Set user password
groupadd hackers            # Create a group
usermod -aG hackers hacker101  # Add user to group

