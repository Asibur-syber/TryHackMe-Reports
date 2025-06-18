# 🌐 ATTACKING WEB APPLICATIONS WITH FFUF – TryHackMe Professional Report

💥 Discover Hidden Web Content | 🛠️ Fuzz like a Pro  
✅ **Room:** Attacking Web Applications with Ffuf  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/ffuf)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

The *Attacking Web Applications with Ffuf* room focuses on using the powerful ffuf tool to discover *hidden directories, files, subdomains*, and *parameters* in web applications.

Understanding and applying fuzzing is essential in real-world penetration testing to uncover attack surfaces that are not visible through normal browsing.

---

## ⚙️ Ffuf Overview

| 🔧 Mode         | 💡 Description                                 |
|----------------|-------------------------------------------------|
| 🗂️ Directory    | Discover hidden folders/files                  |
| 🌐 VHost        | Enumerate virtual hosts (vhosts)               |
| 🔎 Subdomain   | Fuzz subdomains with wordlists                  |
| 📋 Parameter    | Find hidden GET/POST parameters                 |

---

## 🧪 Practical Lab Activities

| 🛠️ Task                       | 🔍 Description                                      |
|------------------------------|-----------------------------------------------------|
| Installed ffuf               | Learned usage and flags                             |
| Directory fuzzing            | Discovered /admin, /backup, and hidden pages    |
| Subdomain fuzzing            | Identified hidden subdomains like dev.site.thm    |
| Parameter fuzzing            | Found vulnerable GET parameters                     |
| Custom wordlist usage        | Used SecLists and crafted personal wordlists        |

---

## 🧾 Sample Fuzzing Commands

```bash
# Basic directory fuzzing
ffuf -u http://10.10.10.10/FUZZ -w /usr/share/wordlists/dirb/common.txt

# Subdomain fuzzing
ffuf -u http://FUZZ.target.thm -H "Host: FUZZ.target.thm" -w subdomains.txt

# GET parameter fuzzing
ffuf -u http://target.thm/index.php?FUZZ=test -w parameters.txt
