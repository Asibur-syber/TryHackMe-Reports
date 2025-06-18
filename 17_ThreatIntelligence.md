# 🧠 THREAT INTELLIGENCE – TryHackMe Professional Report

🛡️ Know Your Enemy | 📡 Gather. Analyze. Defend.  
✅ **Room:** Threat Intelligence  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/threatintel)  
👨‍💻 **Reported by:** Asibur Khan • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** 18-06-2025
5

---

## 🧠 1. Room Overview

The *Threat Intelligence* room teaches how to identify, collect, and use cyber threat information to proactively defend systems. It introduces open-source tools, threat feeds, TTPs (Tactics, Techniques, and Procedures), and the MITRE ATT&CK framework.
🎯 This room helps develop a cyber defender’s mindset — understanding what attackers are doing and how to respond ahead of time.
.

---

## 🧰 2. Tools & Resources Used

- 🌐 *VirusTotal* – File & URL analysis using known threat intel  
- 🛠️ *Shodan* – Search engine for internet-connected devices  
- 🔍 *WHOIS / nslookup / dig* – Investigate domains and IPs  
- 📊 *MITRE ATT&CK* – Framework for understanding adversary behavior  
- 📰 *OSINT Feeds* – Blogs, threat reports, and IOC databases

---

## 🛠️ 3. Key Practical Steps

### 🌐 Step 1: Passive Reconnaissance  
- Used WHOIS to collect domain registration data  
- Analyzed DNS records with nslookup and dig  
- Checked malicious URLs/files using VirusTotal reports  

### 📡 Step 2: Open-Source Intelligence (OSINT)  
- Explored public threat intelligence feeds and databases  
- Gathered IOCs (Indicators of Compromise) from real-world reports  
- Investigated attacker infrastructure via Shodan and Censys  

### 🧠 Step 3: Behavioral Analysis  
- Explored MITRE ATT&CK to map attacker behavior  
- Matched TTPs with discovered indicators  
- Understood how threat intel improves SOC response time

---

## 🏁 4. Flags Captured

- 🎯 Flag 1: THM{PASSIVE_RECON_SUCCESS}  
- 🎯 Flag 2: THM{INTEL_ANALYSIS_COMPLETE}

---

## 🎓 5. Key Takeaways

- ✅ Learned importance of structured threat intel in blue teaming  
- ✅ Practiced recon using real OSINT tools (WHOIS, Shodan, VirusTotal)  
- ✅ Understood how to correlate IOCs with attacker behavior  
- ✅ Explored MITRE ATT&CK matrix for threat classification  

---

## 📸 6. Screenshots (Optional)

![WHOIS Lookup](whois_output.png)  
![MITRE TTP Mapping](mitre_mapping.png)  
![VirusTotal Result](vt_result.png)


---

## 🗒️ 7. Personal Notes

This room built my foundational understanding of threat intel workflows. From passive recon to behavioral mapping, it emphasized how defenders can stay ahead of threats using open intelligence and data correlation.

---

🔚 *End of Report – Asibur Khan*  
🚀 Next: SOC Level 1
