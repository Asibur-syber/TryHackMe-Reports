# 🧑💻 ASIBUR RAHAMAN  
Ethical Hacker | Network Recon Specialist | Red Team Enthusiast  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 📡 TRYHACKME ROOM REPORT — 03: NETWORK FUNDAMENTALS  
🔗 [Room Link → https://tryhackme.com/room/networkfundamentals](https://tryhackme.com/room/networkfundamentals)  
📅 Date Completed: June 28, 2025  
📂 Category: Networking Fundamentals  
🎯 Focus: Subnetting, NAT, DHCP, VPN, Firewalls  
🧩 Difficulty: 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room expands upon basic networking knowledge by diving into five essential components: *Subnetting, DHCP, NAT, VPNs, and Firewalls*. These concepts form the backbone of how modern networks operate and how security is enforced. For ethical hackers and penetration testers, understanding these technologies is critical to identifying vulnerabilities, bypassing restrictions, and safely navigating network environments.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 🔹 1. Subnetting

Subnetting breaks down a large IP network into smaller, manageable blocks.

- *CIDR Notation Example*: 192.168.1.0/24
- *Subnet Mask*: Defines how many bits are allocated to the network
- *Usable Hosts Formula*: 2^host_bits - 2  
  📌 /24 → 255.255.255.0 → 256 total IPs → 254 usable

✅ Helps reduce broadcast traffic, improves segmentation, and adds basic network security.

---

### 📸 Screenshot: Subnetting with ipcalc

[![Subnet Screenshot](https://1drv.ms/i/c/bcf723e80ec8f62e/EeUEsIOm-cZAiVVJON0lz-wBPzFQEkrf0aCBfBbwY2pwgw?e=BLOH5R)](https://1drv.ms/i/c/bcf723e80ec8f62e/EeUEsIOm-cZAiVVJON0lz-wBPzFQEkrf0aCBfBbwY2pwgw?e=BLOH5R)

📌 Command used: ipcalc 192.168.10.0/25  
📌 Result: Shows usable host range from 192.168.10.1 to 192.168.10.126 (126 hosts total)

### 🔹 2. DHCP (Dynamic Host Configuration Protocol)

DHCP servers automatically assign:

- IP Address  
- Subnet Mask  
- Default Gateway  
- DNS Server  

📌 Attackers may set up rogue DHCP servers to inject malicious configurations (like fake DNS).

---

### 🔹 3. NAT (Network Address Translation)

NAT allows devices with private IPs (like 192.168.x.x) to communicate with the internet using a *shared public IP*.

- *Types of NAT*:
  - Static NAT
  - Dynamic NAT
  - Port Address Translation (PAT)

📌 Makes internal network structure invisible to outside attackers; however, understanding NAT helps in pivoting through networks.

---

### 🔹 4. VPN (Virtual Private Network)

VPNs establish a *secure encrypted tunnel* over public or untrusted networks.

- Hides real IP  
- Encrypts data end-to-end  
- Bypasses local firewalls or geo-restrictions

📌 Attackers may use VPNs to hide their identity; organizations use them to secure remote access.

---

### 🔹 5. Firewalls

Firewalls control traffic entering or leaving a system or network based on rules.

- *Types*:
  - Software firewalls: e.g., UFW, Windows Defender  
  - Hardware firewalls: Routers, Gateways  
- Works at *OSI Layers 3 (Network)* and*4 (Transport)**

📌 Understanding how firewalls work allows attackers to find ways around restrictions during exploitation.

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command       | Purpose                                               |
|----------------------|-------------------------------------------------------|
| ipcalc             | Calculate subnets and view CIDR breakdown             |
| ifconfig, ip a   | View current network configuration                    |
| nmap -sn           | Perform ping sweep to discover live hosts             |
| dhclient           | Manually request a DHCP lease                         |
| iptables           | View or set firewall rules on Linux                   |
| traceroute         | Track packet path before/after VPN                    |
| VPN Clients          | OpenVPN, WireGuard for establishing secure tunnels    |

---

## 🖥️ PRACTICAL EXAMPLES

- 🧪 Used ipcalc 192.168.10.0/25 to determine usable IPs  
- 🧪 Ran nmap -sn 192.168.10.0/24 to scan local subnet for live machines  
- 🧪 Requested a DHCP lease viasudo dhclient eth0`  
- 🧪 Set SSH firewall rule with iptables -A INPUT -p tcp --dport 22 -j ACCEPT  
- 🧪 Verified VPN tunnel by comparing traceroute before and after VPN connection  
- 🧪 Compared private (ip a) vs public (curl ifconfig.me) IP for NAT confirmation  

---

## 🔐 SECURITY INSIGHTS

| Topic         | Real-World Relevance to Hacking & Defense                    |
|---------------|--------------------------------------------------------------|
| Subnetting    | Used to segment and isolate critical infrastructure          |
| DHCP          | A common target for *rogue DHCP attacks*                   |
| NAT           | Hides internal IPs, but attackers can still pivot if inside  |
| VPN           | Used to *evade monitoring* or securely access networks     |
| Firewalls     | Detecting, evading, or manipulating firewall rules is common |

---

## 📝 FINAL THOUGHTS

Mastering networking concepts like subnetting, DHCP, NAT, VPNs, and firewalls is crucial for both attackers and defenders. As a penetration tester, these skills allow you to properly *enumerate*, *exploit*, and *bypass protections* in enterprise-grade networks. This room strengthens your ability to assess modern networks effectively.

---

## 🚀 NEXT STEPS

✅ Practice DHCP starvation and rogue server simulations in lab  
✅ Explore iptables rulesets and common misconfigurations  
✅ Prepare for next room: Learn Networking — Understand DNS, MAC Addressing, Packets, and more

---
💡 **"Firewalls, NATs, and VPNs are not obstacles — they are puzzles waiting to be solved."**  
 
— *Asibur Rahaman*
