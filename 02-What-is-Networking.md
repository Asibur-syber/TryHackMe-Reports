# 📡 TryHackMe Room Report — 02: What is Networking

**🔐 Author:** [Asibur Rahaman](https://github.com/Asibur-syber)  
**🌐 Platform:** [TryHackMe](https://tryhackme.com/room/whatisnetworking)  
**📅 Date Completed:** June 27, 2025  
**🏁 Difficulty:** 🟢 Beginner  
**Category:** Networking Fundamentals


---

## 🧠 Room Overview

The "What is Networking" room lays the foundation of modern computer networking for aspiring ethical hackers. It introduces core concepts such as IP addressing, DNS, ports, and the client-server model — skills that every pentester must master.

---

## 🎯 Learning Objectives

- Understand what IP and MAC addresses are
- Learn how DNS resolves human-readable domains into IPs
- Differentiate between TCP and UDP protocols
- Learn what ports are and how services use them
- Use real-world tools to analyze and interact with networks

---

## 🛠️ Tools Used and Practical Commands

| 🧪 Tool        | 🧰 Purpose                                  | ✅ Example Command                          |
|---------------|---------------------------------------------|---------------------------------------------|
| ip a        | Display local IP and interface info         | ip a                                      |
| ping        | Check if a host is alive                    | ping google.com                           |
| nslookup    | DNS lookup for domain-to-IP resolution      | nslookup facebook.com                     |
| telnet      | Manually interact with a service port       | telnet google.com 80                      |
| nmap        | Scan ports and detect service versions      | nmap -sV -Pn scanme.nmap.org              |
| traceroute  | Trace path from source to destination       | traceroute google.com                     |
| whois       | Discover who owns a given IP block          | whois 142.250.195.206                     |

---

## 🔬 Step-by-Step Demonstration

### ✅ 1. Check Local IP Address

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
