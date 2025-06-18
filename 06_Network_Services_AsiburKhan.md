# 🌐 NETWORK SERVICES – TryHackMe Professional Report

🖥️ Discover. Connect. Exploit.  
✅ **Room:** Network Services  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/networkservices)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

In ethical hacking, *network services* are the *entry points* for most attacks. From FTP and SSH to SMB and HTTP — understanding how these services operate allows hackers to *identify misconfigurations*, *leak credentials*, and *escalate privileges*.

This room teaches how to interact with common services, identify vulnerabilities, and exploit them responsibly.
🎯 If you don’t understand services, you’ll miss the attack paths.
.

---

## 🔑 Core Services Covered

| 💻 Service | 🔍 Description                                | 🔓 Common Issues                     |
|------------|-----------------------------------------------|--------------------------------------|
| 🔐 SSH     | Remote secure shell access                    | Weak passwords, outdated versions    |
| 📤 FTP     | File Transfer Protocol                        | Anonymous login, unencrypted traffic |
| 🖥️ SMB     | Windows file sharing (ports 139, 445)         | Null sessions, guest shares          |
| 🌍 HTTP    | Web server communication                      | Directory traversal, outdated CMS    |
| 📡 Telnet  | Insecure remote access (cleartext)            | Password sniffing, outdated service  |
| 📠 SMTP    | Email transfer protocol                       | Open relay, spoofing                 |

---

## 🧪 Lab Skills Practiced

| 🛠️ Tool/Command         | 💼 Purpose                                  |
|--------------------------|---------------------------------------------|
| nmap -sV               | Service and version detection               |
| ftp <IP>               | Manual login to FTP                         |
| enum4linux <IP>        | SMB enumeration                             |
| hydra -l user -P rockyou.txt | Bruteforce FTP/SSH credentials        |
| telnet <IP> 23         | Testing telnet login                        |

---

## ⚙️ Practical Example: FTP Exploitation

```bash
# Connect to FTP server
ftp 10.10.10.10

# Check for anonymous login
Name: anonymous  
Password: <any email>

# If allowed, list and download files
ftp> ls  
ftp> get secrets.txt
