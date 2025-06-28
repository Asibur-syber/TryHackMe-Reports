# 🧑‍💻 ASIBUR RAHAMAN  
*Ethical Hacker | Network Recon Specialist | Red Team Enthusiast*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 📡 TRYHACKME ROOM REPORT — 04: LEARN NETWORKING  
🔗 [Room Link → https://tryhackme.com/room/learnnetworking](https://tryhackme.com/room/learnnetworking)  
📅 *Date Completed:* June 28, 2025  
📂 *Category:* Networking Fundamentals  
🎯 *Focus:* OSI Model, MAC vs IP, Ports, Packet Travel  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room explores the fundamental building blocks of computer networking, such as the *OSI Model*, the distinction between *MAC and IP addresses*, the concept of *ports and protocols*, and how *packets travel* from one host to another. Understanding these concepts is critical for both attackers and defenders in a cybersecurity environment. Without these basics, network reconnaissance, exploitation, or defense cannot be done effectively.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. OSI Model — 7 Layers of Networking

The OSI Model breaks down network communication into 7 layers:

| Layer | Name              | Real-World Example                     |
|-------|-------------------|----------------------------------------|
| 7     | Application       | Web browsers, email (HTTP, SMTP)       |
| 6     | Presentation      | Encryption & encoding (SSL/TLS)        |
| 5     | Session           | Communication setup (NetBIOS, RPC)     |
| 4     | Transport         | TCP/UDP protocols                      |
| 3     | Network           | IP routing, addressing (ICMP, IP)      |
| 2     | Data Link         | MAC addresses, switches                |
| 1     | Physical          | Ethernet cables, NICs, fiber optics    |

🧠 *Importance*: Knowing which layer is involved helps locate misconfigurations or attack surfaces quickly.

---

### 2. MAC Address vs IP Address

- *MAC Address*:  
  - Unique to each network interface  
  - Hardware-based (e.g., 00:1A:2B:3C:4D:5E)  
  - Used within local networks  
  - Layer 2

- *IP Address*:  
  - Logical address for network communication  
  - Can be dynamic (via DHCP)  
  - Used for routing between networks  
  - Layer 3

📌 Hacker Usage: MAC/IP spoofing used to bypass network filters or impersonate devices.

---

### 3. Ports and Protocols

Ports identify services running on devices. Each service listens on a specific port number.

| Service | Port | Protocol |
|---------|------|----------|
| HTTP    | 80   | TCP      |
| HTTPS   | 443  | TCP      |
| SSH     | 22   | TCP      |
| FTP     | 21   | TCP      |
| DNS     | 53   | UDP      |

📌 Key Insight: Port scanning reveals exposed services. Protocol identification helps choose the attack vector.

---

### 4. How Packets Travel (Encapsulation & Decapsulation)

Packets pass through all 7 OSI layers. Each layer adds a "header" to the data:

1. *Application Layer* creates the data  
2. *Transport Layer* splits data into segments (TCP/UDP)  
3. *Network Layer* adds IP address  
4. *Data Link Layer* adds MAC address  
5. *Physical Layer* transmits via cable or Wi-Fi  
6. At receiver’s side, the process is reversed (decapsulation)

🧠 *Understanding packet flow* is essential for tools like Wireshark and for man-in-the-middle attacks.

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command        | Purpose                                              |
|-----------------------|------------------------------------------------------|
| ip a / ifconfig   | Show IP and MAC addresses                            |
| nmap -p             | Scan open ports on target hosts                      |
| traceroute          | View the hop path of packets                         |
| netstat -tuln       | Display listening services and their port bindings   |
| wireshark           | Capture and inspect network packets in detail        |
| ping                | Check ICMP connectivity with hosts                   |

---

## 🖥️ PRACTICAL EXAMPLES

- 🧪 Used ip a to view both MAC and IP of local interface  
- 🧪 Ran nmap -p 1-1000 10.10.10.10 to discover open services  
- 🧪 Analyzed hop count with traceroute tryhackme.com  
- 🧪 Captured TCP handshake with Wireshark to see Layer 4 operations  
- 🧪 Compared encrypted (HTTPS) vs unencrypted (HTTP) traffic using Wireshark  

---

## 🔐 SECURITY INSIGHTS

| Concept         | Security Relevance                                    |
|------------------|------------------------------------------------------|
| OSI Layers       | Identify which layer a vulnerability/attack affects |
| MAC Address      | Can be spoofed for network impersonation             |
| IP Address       | Can be anonymized with VPN/proxy                     |
| Ports & Services | Help attackers find entry points                     |
| Packet Structure | Crucial for MITM/sniffing/data injection             |

---

## 📝 FINAL THOUGHTS

Understanding how networks function at a low level is not optional for ethical hackers — it is mandatory. This room made complex concepts like packet encapsulation, port communication, and addressing systems simple and clear. Mastery of these areas is essential before diving into deeper attack techniques.

---

**"To dominate the network, you must first understand how it speaks."**  
— Asibur Rahaman


---

## 📂 NEXT STEPS

Advance to the next room *“Linux Fundamentals Part 1”* to begin learning core command-line and system management skills needed for penetration testing.

---
