# 🛡️ Professional TryHackMe Report: Nikto Web Server Vulnerability Scanner

*👨‍💻 Prepared by:* Asibur Khan  
*📆 Date:* 19-06-2025  *🌐 Room:** [Nikto on TryHackMe](https://tryhackme.com/room/nikto)  *📂 GitHub Repo:** [TryHackMe-Reports](https://github.com/Asibur-syber/TryHackMe-Reports)

---

## 🔍 1. Executive Summary

Nikto is an essential web server vulnerability scanner used during reconnaissance to detect:
- Outdated server software
- Misconfigured headers
- Dangerous default files
- Known vulnerable scripts

This room helped me understand how to launch *effective Nikto scans*, interpret the results, and prepare high-quality vulnerability assessments.

---

## 🧰 2. Tools & Environment

| Tool     | Functionality                              |
|----------|---------------------------------------------|
| Nikto  | Core web server vulnerability scanner       |
| Kali Linux | Operating system used for testing         |
| Burp Suite (manual verification) | Double-check findings |

---

## 🧪 3. Scanning Strategy & Commands

### 🔹 Basic Nikto Scan:
```bash
nikto -h http://10.10.10.10
```bash
nikto -h http://10.10.10.10:8080
```bash
nikto -h https://10.10.10.10
```bash
nikto -h http://10.10.10.10 -o nikto_report.txt
