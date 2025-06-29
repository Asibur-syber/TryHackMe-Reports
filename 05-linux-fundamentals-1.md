# 🧑‍💻 ASIBUR RAHAMAN  
*Ethical Hacker | Linux Recon Specialist | Terminal Mastermind*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🐧 TRYHACKME ROOM REPORT — 05: LINUX FUNDAMENTALS 1  
🔗 [Room Link → https://tryhackme.com/room/linuxfundamentals1](https://tryhackme.com/room/linuxfundamentals1)  
📅 *Date Completed:* June 28, 2025  
📂 *Category:* Operating System (Linux Basics)  
🎯 *Focus:* File System Navigation, Commands, Shell Basics  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room introduces users to the *Linux operating system*, which powers most servers, hacking labs, and cybersecurity tools. The room explains essential concepts such as *file system structure*, *basic terminal commands*, *permissions*, and *file handling*. These skills are foundational for ethical hackers, system administrators, and penetration testers.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. What is Linux?

- Linux is a *UNIX-like open-source OS* used in servers, hacking labs, and embedded systems.
- It provides a *terminal-based environment* for direct system control.

📌 Hacker Insight: Most pentesting machines and tools (like Kali Linux) are Linux-based.

---

### 2. Linux File System Structure

Linux uses a *hierarchical file system* starting from / (root). Key directories:

| Directory | Purpose |
|----------|---------|
| /home  | User files and directories |
| /etc   | Configuration files |
| /bin   | Essential binary commands |
| /var   | Logs, spools |
| /root  | Root user’s home |
| /tmp   | Temporary files |

📌 Understanding these helps when exploiting misconfigurations or privilege escalation paths.

---

### 3. Navigating with the Terminal

| Command        | Use                              |
|----------------|-----------------------------------|
| pwd          | Show current directory            |
| ls           | List files/folders                |
| cd /path     | Change directory                  |
| clear        | Clear terminal                    |
| file name    | Show file type                    |

🧠 Every pentester must be comfortable with navigating the Linux file system from the command line.

---

### 4. Working with Files and Directories

| Command                        | Description                          |
|--------------------------------|--------------------------------------|
| touch file.txt              | Create a file                        |
| mkdir folder                | Create a directory                   |
| cat file.txt                | Display file content                 |
| rm file.txt                 | Delete a file                        |
| rmdir folder                | Remove a directory                   |
| cp src dest                 | Copy files/folders                   |
| mv old new                  | Move or rename files/folders         |

📌 Common during exploitation when accessing config files or uploading payloads.

---

### 5. Understanding Linux Shells

- *Shell* is the interface between user and OS (e.g., Bash, Zsh).
- Commands are interpreted via shell scripting.

📌 Reverse shells rely on understanding how Linux interprets commands.

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command    | Purpose                                 |
|-------------------|-----------------------------------------|
| pwd, ls, cd | Navigation                              |
| touch, mkdir  | Create files and folders                |
| rm, rmdir     | Remove files/folders                    |
| cat, file     | View and inspect files                  |
| whoami, id    | Check current user and permissions      |
| man <command>   | View manual page for any command        |

---

## 🖥️ PRACTICAL EXAMPLES

- 🧪 Used cd /etc && ls to explore configuration files  
- 🧪 Ran touch test.txt and cat test.txt to create and view a file  
- 🧪 Verified current user with whoami andid`  
- 🧪 Used mkdir tools && cd tools to prepare a working directory  
- 🧪 Used file command on a binary to identify its type  
- 🧪 Used man ls to learn about listing options (e.g.,ls -la`)

---

## 🔐 SECURITY INSIGHTS

| Concept          | Relevance to Security                                |
|------------------|------------------------------------------------------|
| File Permissions | Improper settings may allow privilege escalation     |
| Terminal Access  | Attackers use CLI to upload, modify, or delete files |
| Shells           | Exploits often deliver reverse/bind shells           |
| File System      | Malware often hides in /tmp, misused /etc        |

---

## 📝 FINAL THOUGHTS

Mastering the Linux terminal is like learning the *language of hackers*. This room lays the foundation for *post-exploitation*, *privilege escalation*, and *red team operations*. From enumeration to maintaining access, Linux comm
