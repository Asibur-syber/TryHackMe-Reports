# 🧑‍💻 ASIBUR RAHAMAN  
*Ethical Hacker | Network Recon Specialist | Red Team Enthusiast*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 📡 TRYHACKME ROOM REPORT — 02: WHAT IS NETWORKING  
🔗 [Room Link → https://tryhackme.com/room/whatisnetworking](https://tryhackme.com/room/whatisnetworking)  
📅 *Date Completed:* June 27, 2025  
📂 *Category:* Networking Fundamentals  
🎯 *Focus:* IP Address, DNS, Ports, Protocols, OSI Model  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room introduces the foundational concepts of networking critical for ethical hackers. It covers how devices communicate over a network, the importance of IP addresses, DNS translation, ports for different services, networking protocols like TCP and UDP, and the OSI model layers. Mastering these basics is essential before moving on to active scanning and exploitation in penetration testing.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. What is Networking?

Networking is the process by which multiple devices (computers, phones, routers) exchange data. Communication happens via wired or wireless connections enabling services like browsing and messaging.

---

### 2. IP Address

An IP address is a unique identifier for each device on a network. There are two types:
- *Private IP:* Used inside local networks (e.g., 192.168.1.5)
- *Public IP:* Used on the internet (provided by ISP)

Understanding IPs is vital for network mapping and attacks.

---

### 3. DNS (Domain Name System)

Humans use domain names (e.g., google.com), but computers use IP addresses. DNS translates domain names into IPs, allowing us to access websites easily.

---

### 4. Ports

Ports act as communication endpoints for services on a device:
- HTTP runs on port 80
- HTTPS on port 443
- SSH on port 22

Each port number corresponds to a specific service.

---

### 5. Protocols: TCP vs UDP

- *TCP* is connection-oriented and reliable — ensures data delivery.
- *UDP* is faster but connectionless and does not guarantee delivery.

---

### 6. OSI Model

The OSI model defines 7 layers describing how data travels from one device to another:
1. Physical  
2. Data Link  
3. Network  
4. Transport  
5. Session  
6. Presentation  
7. Application  

Understanding this helps in troubleshooting and security analysis.

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command | Purpose                               |
|----------------|-------------------------------------|
| ip a         | Check local IP address               |
| ping         | Test if a host is reachable          |
| nslookup     | Resolve domain name to IP address   |
| telnet       | Test connectivity to a port          |
| nmap         | Scan open ports and services         |
| traceroute   | Trace path packets take to a host    |
| whois        | Find ownership information of IP    |

---

## 🖥️ PRACTICAL EXAMPLES

- Checked local IP using ip a  
- Pinged google.com with ping google.com to verify connectivity  
- Resolved facebook.com IP with nslookup facebook.com  
- Tested HTTP port using telnet facebook.com 80 and verified server response  
- Scanned ports on Facebook IP using nmap -sV -Pn 157.240.25.35  
- Traced route to Google using traceroute google.com  
- Retrieved IP ownership via whois 142.250.195.206

---

## 📝 FINAL THOUGHTS

Networking forms the backbone of all cybersecurity operations. Thorough knowledge of IP addresses, DNS, ports, protocols, and the OSI model equips ethical hackers with the essential skills to perform reconnaissance and prepare for exploitation effectively.

---

**“Understanding networking is the first step towards mastering cybersecurity.”**  
— Asibur Rahaman


---

## 📂 NEXT STEPS

Proceed to the next room *“Network Fundamentals”* to dive deeper into subnetting, DHCP, NAT, and VPN concepts.

---

## 🔬 Step-by-Step Demonstration

✅ 1. Check Local IP Address

```bash
ip a

✅ 2. Test External Server Availability

```bash

ping google.com

✅ 3. Resolve Domain Name to IP

```bash

nslookup facebook.com

✅ 4. Interact With Web Server Over HTTP Port

```bash

telnet google.com 80

```bash

GET / HTTP/1.1
Host: google.com

✅ 5. Scan for Open Ports and Services

```bash

nmap -sV -Pn scanme.nmap.org

✅ 6. Trace Route to Target

```bash

traceroute google.com

✅ 7. Perform Whois Lookup

whois 142.250.195.206
