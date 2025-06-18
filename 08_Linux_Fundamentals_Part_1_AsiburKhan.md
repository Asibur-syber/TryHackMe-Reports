# 🐧 LINUX FUNDAMENTALS PART 1 – TryHackMe Professional Report

💡 From Shell to Root – Start your Linux Hacking Journey  
✅ **Room:** Linux Fundamentals Part 1  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/linuxfundamentals1)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

Linux is the foundation of most hacking environments — including *Kali Linux* and almost every server in the cloud. This room builds a strong base in understanding Linux systems, commands, file structures, and user roles.
🚀 Whether you're hacking, scripting, or administering — **Linux is essential.**
*

---

## 🧠 Key Concepts Learned

| 🔧 Topic                   | 📚 Description                                             |
|---------------------------|------------------------------------------------------------|
| 🐧 Linux Distributions     | Debian, Ubuntu, Kali – Different flavors, one core        |
| 📁 File System Hierarchy   | /bin, /etc, /home, /root, /var explained                  |
| 🧑‍💻 User vs Root Access     | sudo for superpower – never run as root unless needed |
| 🗃️ File Operations         | ls, cd, cp, mv, rm, touch, mkdir            |
| 📑 Viewing Files           | cat, less, more, head, tail                     |
| 🧭 Navigation              | pwd, cd .., cd /, clear                           |

---

## 🛠️ Command Practice Examples

### 📂 Basic File Navigation

```bash
pwd            # Show current directory
ls -la         # List all files with permissions
cd /etc        # Move into /etc directory
touch hello.txt            # Create a new file
echo "Asibur Rocks!" > a.txt  # Add content to file
cat a.txt                  # View contents
whoami         # Show current user
sudo su        # Switch to root (if permitted)
id             # Show UID/GID and groups
