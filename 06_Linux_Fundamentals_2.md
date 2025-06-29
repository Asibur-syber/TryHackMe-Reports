# 🧑‍💻 ASIBUR RAHAMAN  
*Ethical Hacker | Linux Recon Specialist | Terminal Mastermind*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🐧 TRYHACKME ROOM REPORT — 06: LINUX FUNDAMENTALS 2  
🔗 [Room Link → https://tryhackme.com/room/linuxfundamentals2](https://tryhackme.com/room/linuxfundamentals2)  
📅 *Date Completed:* June 29, 2025  
📂 *Category:* Operating System (Linux Basics)  
🎯 *Focus:* File Permissions, File Editing, Searching, Process Management  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room expands upon basic Linux usage by focusing on *file permissions*, **file editing tools (like nano)**, *searching files*, and *managing processes*. These are critical skills in system administration, scripting, and ethical hacking — especially during *post-exploitation*, *privilege escalation*, and *maintaining access*.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. Linux File Permissions (rwx)

Each file/directory has three types of access:

| Permission | Meaning        |
|------------|----------------|
| r        | Read           |
| w        | Write          |
| x        | Execute        |

Permissions are divided among:

- *User (u)* – owner  
- *Group (g)* – group members  
- *Others (o)* – everyone else

🧠 View permissions usingls -l`  
🛠 Modify permissions using chmod, chown
chgrp`

📌 Hacker Note: Weak file permissions can allow privilege escalation or data leaks.

---

### 2. Editing Files with Nano

- nano is a *CLI text editor*.
- Used to view and edit configuration files, scripts, etc.

🛠 Commands inside nano:
- Ctrl+O → Save  
- Ctrl+X → Exit  
- Ctrl+K → Cut Line  
- Ctrl+U → Paste Line  

📌 Used in real-world pentesting to modify cron jobs, scripts, or inject reverse shells.

---

### 3. Searching with find and grep

| Command Example         | Description            |
|------------------------|------------------------|
| find / -name passwd   | Search for a file by name |
| grep root /etc/passwd | Search for text in a file |

🧠 find searches the file system  
🧠 grep searches inside files  

📌 Privilege escalation often uses these to discover misconfigurations or sensitive info.

---

### 4. Managing Processes with ps, top, kill

| Command         | Purpose                       |
|-----------------|-------------------------------|
| ps aux        | Show all running processes    |
| top           | Live view of CPU/memory usage |
| kill <PID>    | Stop a process by PID         |

📌 During post-exploitation, these help monitor or kill unwanted detection agents.

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command     | Purpose                                 |
|--------------------|-----------------------------------------|
| ls -l            | View file permissions                   |
| chmod +x file    | Add execute permission                  |
| chown user file  | Change file ownership                   |
| nano file.txt    | Edit file using Nano editor             |
| `find / -name file`| Search file by name                     |
| `grep keyword file`| Search keyword inside file              |
| ps aux           | List all running processes              |
| kill <PID>       | Terminate a running process             |

---

## 🖥️ PRACTICAL EXAMPLES

- 🧪 Used chmod 755 script.sh to make a script executable  
- 🧪 Edited notes.txt using nano and saved changes  
- 🧪 Found hidden password file using find / -name secret.txt  
- 🧪 Searched for keywords with grep 'password' config.txt  
- 🧪 Killed a suspicious process withkill 3245`  

---

## 🔐 SECURITY INSIGHTS

| Topic               | Relevance to Hacking                         |
|---------------------|----------------------------------------------|
| File Permissions    | Weak settings → Lateral movement / Escalation |
| File Searching      | Used to find creds, config, backup files     |
| Process Control     | Used to kill AV, loggers, or maintain stealth|

---

## 📝 FINAL THOUGHTS

This room teaches the *hands-on controls* every ethical hacker needs when operating inside a Linux system. After exploitation, hackers often use nano, find, chmod, and ps to *plant payloads*, *change permissions*, or *extract information*.  
🧠 Mastering these tools is essential for anyone aiming to dominate Linux-based environments.
.

---

## 🚀 NEXT STEPS

- ✅ Proceed to*Linux Fundamentals 3**  
- 🧠 Practice using chmod
chown` on test files  
- 🔍 Explore grep + find to scan large directories quickly  
- 🛠 Learn about cron jobs and file automation  
- 📘 Start building your own Linux cheat sheet

---
💡 “The true hacker isn’t afraid of the terminal — they *live* in it.” – ASIBUR RAHAMAN
N

---
