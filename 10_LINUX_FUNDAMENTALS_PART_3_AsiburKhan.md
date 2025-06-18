# 🐧 LINUX FUNDAMENTALS – PART 3 – TryHackMe Professional Report

🧠 Learn. 🔍 Practice. 💻 Hack.  
✅ **Room:** Linux Fundamentals Part 3  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

Building upon the basics, this room guides learners through advanced Linux user and permission management concepts. Mastering these ensures a strong foundation for securing Linux systems and conducting effective penetration tests.
🎯 **Goal:** Equip yourself with the skills to confidently manage Linux users, control file permissions, and utilize sudo for administrative tasks.
.

---

## 📚 What You Will Learn

| 🔹 Topic                  | 🔎 Description                                                |
|--------------------------|--------------------------------------------------------------|
| 👤 User & Group Management | How to create, modify, and delete users and groups           |
| 🏷️ File Ownership          | Assigning and changing file owners and groups                |
| 🔐 Permission Schemes      | Understanding and applying read, write, and execute rights  |
| ⚡ Sudo Privileges         | Running commands with elevated rights securely               |

---

## 🛠️ Essential Commands & Concepts

### User & Group Management

```bash
sudo adduser <username>         # Create a new user
sudo deluser <username>         # Remove a user
sudo usermod -aG <group> <user> # Add user to a group
cat /etc/passwd                 # User account info
cat /etc/group                  # Group info

```bash
ls -l                          # View file owner and permissions
sudo chown <user>:<group> <file>  # Change owner and group
sudo chmod 755 <file>          # Set rwxr-xr-x permissions

```bash
sudo <command>                 # Execute command as root
sudo visudo                   # Safely edit sudoers file
