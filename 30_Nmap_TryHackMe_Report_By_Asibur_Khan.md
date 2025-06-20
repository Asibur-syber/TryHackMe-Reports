# 📡 TryHackMe Report: Nmap - Network Scanning Mastery

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [Nmap on TryHackMe](https://tryhackme.com/room/nmap)

---

## 🧠 1. Room Summary:

This room teaches how to master *Nmap*, the most powerful network scanning tool used by ethical hackers.  
I learned how to scan networks, detect open ports, identify services, and find operating system info — all of which are essential for pre-attack reconnaissance.

---

## 🛠️ 2. Tools Used:

| Tool  | Purpose                            |
|-------|------------------------------------|
| nmap | Port scanning, service discovery  |

---

## 🚀 3. Exploitation & Scanning Steps

### 🔍 Step 1: Basic Port Scan
```bash
nmap 10.10.10.10
```bash
nmap -sV 10.10.10.10
```bash
nmap -A 10.10.10.10
```bash
nmap -O 10.10.10.10
```bash
nmap -p 80,443 --script http-enum 10.10.10.10
