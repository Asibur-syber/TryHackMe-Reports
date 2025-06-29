# 🧑‍💻 ASIBUR RAHAMAN  
*Ethical Hacker | Linux Recon Specialist | Terminal Mastermind*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🐧 TRYHACKME ROOM REPORT — 05: LINUX FUNDAMENTALS 1  
🔗 [Room Link → https://tryhackme.com/room/linuxfundamentals1](https://tryhackme.com/room/linuxfundamentals1)  
📅 *Date Completed:* June 29, 2025  
📂 *Category:* Linux Basics  
🎯 *Focus:* Terminal Navigation, File Management, Permissions, Wildcards, Text Editing  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This TryHackMe room introduces foundational Linux terminal commands and system usage. For ethical hackers, this knowledge is essential to move within a target system, manipulate files, escalate privileges, and automate tasks using shell commands.

Topics covered include:

- Navigating file systems
- Managing files and directories
- File permissions and chmod
- Using wildcards for flexible matching
- Editing files with nano

Mastering these fundamentals builds a strong base for Linux privilege escalation and exploitation.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. Filesystem Navigation

| Command     | Description                           |
|-------------|---------------------------------------|
| pwd       | Show current directory path           |
| ls        | List files and folders in directory   |
| `cd folder/`| Enter a folder                        |
| cd ..     | Go one level back                     |
| cd /      | Move to root directory                |
| cd ~      | Move to home directory                |

---

### 2. Creating & Managing Files and Directories

| Command                         | Description                         |
|---------------------------------|-------------------------------------|
| touch filename.txt            | Create an empty file                |
| mkdir foldername              | Create a new folder                 |
| mv old new                    | Rename or move file/folder          |
| cp source dest                | Copy file/folder                    |
| rm file.txt                   | Remove a file                       |
| rm -r folder/                 | Remove a folder and contents        |

---

### 3. Understanding Permissions & chmod

Each file has 3 types of users:
- *User (u)* — Owner
- *Group (g)* — Assigned group
- *Others (o)* — Everyone else

Each user type can have:
- *r*: Read
- *w*: Write
- *x*: Execute

To view permissions:
```bash
ls -l

To change permissions:

chmod 755 file.sh   # User: rwx, Group: rx, Others: rx
chmod u+x script.sh # Add execute to owner

Value	Permission	Binary Meaning

777	rwxrwxrwx	All: full access
755	rwxr-xr-x	Common for scripts
644	rw-r--r--	Files: read/write



---

### 4. Wildcards

Wildcards help with multiple files:

Wildcard	Description	Example

*	Matches any string	ls *.txt
?	Matches one character	ls file?.txt



---

### 5. Editing Files Using nano

nano is a lightweight terminal text editor.

Shortcut	Function

Ctrl + O	Save the file
Ctrl + X	Exit editor
Ctrl + K	Cut a line
Ctrl + U	Paste a line


Example:

nano readme.txt
# Inside nano: Write some text


---

### 🧰 TOOLS & COMMANDS USED

Tool / Command	Purpose

pwd	Print current working directory
ls, ls -l	List directory contents
cd, cd ..	Navigate directories
mkdir, touch	Create folders and files
mv, cp, rm	Move, copy, and remove files/folders
chmod	Change file permission
nano	Terminal text editor
*, ?	Wildcard usage for flexible matching



---

### 🖥️ PRACTICAL EXAMPLES

Here are real commands executed during the lab:

cd ~
mkdir THM
cd THM
touch report.txt
nano report.txt

Inside nano, typed:

Hello from Linux Fundamentals!

Then ran:

cp report.txt backup.txt
mv backup.txt final.txt
chmod 755 final.txt
ls -l *.txt

## 📥 Output:

-rwxr-xr-x 1 asibur asibur 31 Jun 29 12:12 final.txt
-rw-r--r-- 1 asibur asibur 31 Jun 29 12:11 report.txt


---

### 📝 FINAL THOUGHTS

Linux is at the heart of cybersecurity. Knowing terminal commands allows ethical hackers to:

Move through systems invisibly

Handle sensitive files

Bypass permission barriers

Automate tasks with scripts


This room teaches practical Linux usage that directly helps in real-world hacking.


---

"Before you can hack the system, you must first command the terminal."



---

### 📂 NEXT STEPS

➡️ Move to the next room Linux Fundamentals Part 2 to learn:

User & group management

File ownership with chown

Process and service monitoring

Linux privilege enumeration
