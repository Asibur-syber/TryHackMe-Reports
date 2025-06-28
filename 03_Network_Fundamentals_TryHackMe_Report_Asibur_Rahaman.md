# 🧑‍💻 ASIBUR RAHAMAN  
*Ethical Hacker | Network Recon Specialist | Red Team Enthusiast*  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 📡 TRYHACKME ROOM REPORT — 03: NETWORK FUNDAMENTALS  
🔗 [Room Link → https://tryhackme.com/room/networkfundamentals](https://tryhackme.com/room/networkfundamentals)  
📅 *Date Completed:* June 28, 2025  
📂 *Category:* Networking Fundamentals  
🎯 *Focus:* Subnetting, NAT, DHCP, VPN, Firewalls  
🧩 *Difficulty:* 🟢 Beginner  

---

## 🧠 EXECUTIVE SUMMARY

This room continues building a strong foundation in networking by diving into more advanced concepts essential for ethical hacking. It explains how IP addressing works in subnetted networks, how DHCP automates network configurations, the role of NAT in IP translation, the function of VPNs for secure communication, and how firewalls protect networks from unauthorized access. Each topic is crucial for understanding how networks operate, and how attackers can navigate or bypass defenses.

---

## 🎯 WHAT I LEARNED (STEP-BY-STEP)

---

### 1. Subnetting

Subnetting divides a large network into smaller segments for better management and security.

- *CIDR Notation*: Example — 192.168.1.0/24
- *Subnet Mask*: Determines the number of usable hosts
- *Why it's important*: Helps in organizing IPs and reducing broadcast traffic

🧮 *Formula Example:*  
/24 → 255.255.255.0 → 256 IPs total → 254 usable hosts

---

### 2. DHCP (Dynamic Host Configuration Protocol)

DHCP dynamically assigns IP addresses, gateway, DNS, and subnet mask to clients.

- Reduces manual configuration
- In real networks, DHCP is often a key point of attack (e.g., rogue DHCP)

---

### 3. NAT (Network Address Translation)

NAT allows multiple devices with *private IPs* to access the internet via a *single public IP*.

- Used in routers and firewalls
- Essential for IPv4 address conservation
- *Types:* Static NAT, Dynamic NAT, Port Address Translation (PAT)

---

### 4. VPN (Virtual Private Network)

VPNs create a *secure, encrypted tunnel* between the user and the destination.

- Prevents packet sniffing and man-in-the-middle attacks
- Hides original IP address
- Example: OpenVPN, WireGuard

---

### 5. Firewalls

Firewalls filter incoming and outgoing traffic based on pre-defined rules.

- Types: *Software* (Windows Defender), *Hardware* (router firewalls)
- Works on OSI Layers 3 and 4
- Can *allow/deny ports, IPs, protocols*

---

## 🧰 TOOLS & COMMANDS USED

| Tool / Command       | Purpose                                             |
|----------------------|-----------------------------------------------------|
| ipcalc             | Calculate subnets and CIDR                         |
| ifconfig / ip a  | Check IP configuration                             |
| nmap -sn           | Discover live hosts in a subnet                    |
| dhclient           | Request DHCP lease manually                        |
| iptables           | View/manage Linux firewall rules                   |
| traceroute         | Analyze route with/without VPN                     |
| VPN Tools            | OpenVPN, WireGuard for secure tunneling            |

---

## 🖥️ PRACTICAL EXAMPLES

- Used ipcalc 192.168.10.0/25 to determine subnets  
- Ran nmap -sn 192.168.10.0/24 to identify live machines on local subnet  
- Configured and requested IP from DHCP using dhclient eth0  
- Set firewall rules using iptables -A INPUT -p tcp --dport 22 -j ACCEPT  
- Connected via VPN and compared traceroute path before and after  
- Verified NAT effect by comparing ip a private IP vs curl ifconfig.me public IP  

---

## 🔐 SECURITY INSIGHTS

| Concept        | How Hackers Use It / Protect Against It                  |
|----------------|---------------------------------------------------------|
| Subnetting     | Helps isolate targets; scanning gets complex             |
| DHCP           | Attackers can setup rogue DHCP to assign malicious DNS  |
| NAT            | Obscures internal structure; attackers must pivot        |
| VPN            | Protects against traffic sniffing on public networks     |
| Firewalls      | Detect & evade firewall rules during exploitation        |

---

## 📝 FINAL THOUGHTS

Understanding subnetting, DHCP, NAT, VPNs, and firewalls is fundamental for penetration testers. These concepts shape how real-world networks are structured and defended. Mastery of these areas ensures that you can operate within complex infrastructures, bypass limitations, and execute successful assessments.

---

**"Firewalls, NATs, and VPNs are not obstacles — they are puzzles waiting to be solved."**  
— Asibur Rahaman


---

## 📂 NEXT STEPS

Advance to the next room *“Intro to LAN”* to start learning about ARP, switches, and man-in-the-middle attacks within a local area network.

---
