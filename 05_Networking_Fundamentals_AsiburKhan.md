# 🌐 NETWORKING FUNDAMENTALS – TryHackMe Professional Report

📡 Backbone of Cybersecurity | 💻 Understand before you Hack  
✅ **Room:** Networking Fundamentals  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/networkingfundamentals)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

Networking is the *foundation* of everything in cybersecurity. Without understanding how devices communicate, how IP addresses work, or what a port is — it’s impossible to hack, defend, or investigate systems effectively.

This TryHackMe room introduces the *core concepts of networking* from a cybersecurity perspective: IP, DNS, TCP/IP, ports, protocols, and how data flows across the internet.
🎯 Learn how attackers use this knowledge — and how defenders secure systems against misuse.
.

---

## 🔑 Key Concepts Covered

| 🔸 Topic             | 🔍 Description                                                                 |
|----------------------|--------------------------------------------------------------------------------|
| 📍 IP Address        | Unique identifier for every device on a network (IPv4 & IPv6)                  |
| 🌐 DNS               | Resolves domain names to IP addresses (like a phonebook for the internet)      |
| 📦 TCP/UDP           | Transport layer protocols: TCP = reliable, UDP = fast                          |
| 🚪 Ports             | Logical access points on a device (e.g., port 80 = HTTP)                       |
| 🎯 ICMP & Ping       | Used for testing network reachability                                          |
| 📡 Routing & Subnetting | Determines how data finds its destination                                 |

---

## 🧪 Lab Activities Overview

| 🛠️ Activity                    | 💻 What You Did                                 |
|-------------------------------|--------------------------------------------------|
| ip a & ifconfig           | Check your system’s IP address                  |
| ping, traceroute          | Test reachability & path of packets             |
| nslookup, dig             | Discover IP from domain (DNS lookup)            |
| netstat, ss               | See open connections & listening ports          |
| nmap                        | Scan a target’s IP & ports                      |

---

## 🌐 Protocols You Learned

| 📡 Protocol | 🔍 Function                                | 🔒 Security Relevance                       |
|-------------|---------------------------------------------|---------------------------------------------|
| HTTP/HTTPS  | Web communication (unencrypted/encrypted)   | HTTPS protects confidentiality              |
| DNS         | Resolves domains                            | DNS spoofing is a common attack vector      |
| ICMP        | Network diagnostics                         | Used in ping sweeps, DDoS                   |
| TCP/UDP     | Reliable vs. fast transmission              | Port scanning abuses TCP/UDP behaviors      |

---

## 📈 Sample Terminal Outputs

```bash
# Check IP Address
ip a

# Ping a website
ping google.com

# DNS Lookup
nslookup tryhackme.com

# Port Scan with Nmap
nmap -sS -Pn 10.10.10.10
