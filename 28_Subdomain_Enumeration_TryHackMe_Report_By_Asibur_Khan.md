# 🌐 TryHackMe Report: Subdomain Enumeration

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [Subdomain Enumeration on TryHackMe](https://tryhackme.com/room/subdomainenumeration)

---

## 🧠 1. Room Overview

This room focuses on *Subdomain Enumeration*, a crucial reconnaissance step in penetration testing to discover hidden or forgotten subdomains of a target domain.  
Identifying subdomains helps map the full attack surface and find potential vulnerabilities.

---

## 🛠️ 2. Tools & Techniques Used

| Tool           | Purpose                                  |
|----------------|-------------------------------------------|
| Sublist3r    | Fast subdomain enumeration                |
| Amass        | Advanced subdomain discovery and mapping  |
| crt.sh       | Certificate transparency logs lookup     |
| dig          | DNS queries and manual verification       |

---

## 🚀 3. Step-by-Step Process

### Step 1: Automated Enumeration with Sublist3r
- Ran sublist3r to gather initial list of subdomains.  
  ```bash
  sublist3r -d target.com
  ```bash
  amass enum -d target.com
  ```bash
  dig subdomain.target.com
