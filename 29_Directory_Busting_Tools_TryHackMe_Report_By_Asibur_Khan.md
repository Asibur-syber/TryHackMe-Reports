# 🗂️ TryHackMe Report: Directory Busting Tools – Dirb | Gobuster | Dirbuster

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room Link:* [TryHackMe - Directory Busting](https://tryhackme.com/room/directorybusting)

---

## 🧠 1. Room Summary:

In this room, I learned how to use three powerful tools — *Dirb*, *Dirbuster*, and *Gobuster* — to discover hidden directories and sensitive files on web servers.  
These tools are essential for finding unlisted admin panels, backups, upload points, and other exposed paths that could lead to serious vulnerabilities.

---

## 🧪 2. Tools Used:

| Tool        | Role                                      |
|-------------|-------------------------------------------|
| *Dirb*     | Basic directory brute-forcing using wordlists |
| **Dirbuster**| Recursive GUI-based path discovery        |
| *Gobuster* | Fast and efficient directory scanning      |

---

## 💣 3. Exploitation Steps:

### 🔍 Step 1: Dirb – Initial Scan
```bash
dirb http://target.com /usr/share/wordlists/dirb/common.txt
```bash
gobuster dir -u http://target.com -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -t 50
