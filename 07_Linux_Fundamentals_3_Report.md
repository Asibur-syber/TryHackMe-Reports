# 🧑💻 ASIBUR RAHAMAN  
**Ethical Hacker | Linux Recon Specialist | Terminal Mastermind**  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🐧 TRYHACKME ROOM REPORT — 07: LINUX FUNDAMENTALS 3  
🔗 [Room Link → https://tryhackme.com/room/linuxfundamentals3](https://tryhackme.com/room/linuxfundamentals3)  
📅 **Date Completed:** July 1, 2025  
📂 **Category:** Operating System (Linux Basics)  
🎯 **Focus:** File Permissions, Users & Groups, File Redirection, Environment Variables  
🧩 **Difficulty:** 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room completes the foundational journey into Linux by diving into **permissions, user/group management, input/output redirection, and environment variables**. These concepts are **essential for privilege escalation, secure configuration, and exploiting misconfigurations** in real-world ethical hacking. Understanding how Linux handles user roles and permission hierarchies is key to any serious pentester.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. File & Directory Permissions

Linux permissions follow the format: `-rwxr-xr--`  
- Each file/directory has 3 permission sets: **Owner, Group, Others**
- Permissions:  
  - `r` = read  
  - `w` = write  
  - `x` = execute  

Use `ls -l` to see permissions and ownership.

📌 *Understanding this is critical in privilege escalation and post-exploitation.*

---

### 2. Changing Permissions with `chmod`

| Command               | Purpose                        |
|------------------------|-------------------------------|
| `chmod +x script.sh`   | Add execute permission         |
| `chmod 755 filename`   | Set specific permission bits   |

Numeric permission breakdown:  
- `7` = `rwx`  
- `6` = `rw-`  
- `5` = `r-x`, etc.

🧠 *Used to make exploit scripts executable or modify access on vulnerable files.*

---

### 3. Ownership with `chown`

| Command                        | Description                             |
|--------------------------------|-----------------------------------------|
| `chown user:group filename`    | Change file owner and group             |
| `sudo chown root:root file`    | Set ownership to root (admin)           |

📌 *Used often to restrict or elevate control over sensitive files.*

---

### 4. Users and Groups

| Command           | Use                                    |
|-------------------|----------------------------------------|
| `whoami`          | Display current user                   |
| `id`              | Show user ID and group info            |
| `adduser <name>`  | Add a user                             |
| `usermod -aG`     | Add user to a group                    |
| `groups`          | Show user’s group memberships          |

📌 *Essential for managing multi-user environments, access control, and user privilege analysis.*

---

### 5. Input/Output Redirection

| Symbol     | Function                        |
|------------|---------------------------------|
| `>`        | Redirect output to a file       |
| `>>`       | Append output to a file         |
| `<`        | Input from file                 |
| `|` (pipe) | Send output to another command  |

Examples:  
- `echo hello > file.txt`  
- `cat file.txt | grep admin`

🧠 *Redirection is often used in automation and command chaining during enumeration.*

---

### 6. Environment Variables

- Stored data available to all processes in a session
- Example: `$PATH`, `$HOME`, `$USER`, etc.
- Set using: `export VAR=value`

📌 *Attackers often modify PATH or leverage environment variables to hijack execution paths.*

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command       | Purpose                                         |
|----------------------|-------------------------------------------------|
| `ls -l`              | View file permissions and ownership             |
| `chmod`, `chown`     | Modify file permissions and ownership           |
| `whoami`, `id`       | Check user identity and groups                  |
| `adduser`, `usermod` | Manage system users and groups                  |
| `echo`, `cat`, `>`   | Redirect and view input/output                  |
| `export`, `printenv` | Manage and display environment variables        |
| `groups`, `su`, `sudo` | Switch user, gain elevated access             |

---

## 🖥️ PRACTICAL EXAMPLES

- 🧪 Used `chmod +x exploit.sh` to make a script executable  
- 🧪 Modified a file’s owner with `chown asibur:asibur target.txt`  
- 🧪 Created a user with `sudo adduser testuser`  
- 🧪 Appended output using `echo "new log" >> logs.txt`  
- 🧪 Changed PATH variable temporarily using `export PATH=~/scripts:$PATH`  
- 🧪 Used `whoami` inside an exploit to confirm session privileges  

---

## 🔐 SECURITY INSIGHTS

| Topic                 | Security Impact                                                 |
|-----------------------|-----------------------------------------------------------------|
| File Permissions      | Weak settings can lead to unauthorized read/write/exec access   |
| User Management       | Misconfigured users can be abused for privilege escalation      |
| Redirection & Pipes   | Used in chained payload delivery and command injection attacks  |
| Environment Variables | PATH hijacking or misused variables can lead to exploitation    |

---

## 📝 FINAL THOUGHTS

Linux Fundamentals 3 gives **deep control-level understanding** of how Linux enforces access control, manages users, and handles command inputs. These skills are directly applied in **CTFs, real-world engagements**, and **post-exploitation scenarios**. Knowing how to manipulate user/group settings and permissions is a core weapon in an ethical hacker’s arsenal.

---

## 🚀 NEXT STEPS

✅ Practice permission modification and PATH hijacking in labs  
✅ Study SUID/SGID files and privilege escalation vectors 

---

> 💡 **“Access is not always gained through force — sometimes, it's a permission left unchecked.”**  
> — *Asibur Rahaman*
