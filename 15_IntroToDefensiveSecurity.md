# 🛡️ INTRO TO DEFENSIVE SECURITY – TryHackMe Professional Report

🔐 Defend. Detect. Respond. | 🧠 Understand how Blue Teams Operate  
✅ **Room:** Intro to Defensive Security  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/introtodefensivesecurity)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

Defensive Security focuses on protecting systems against attackers by using tools, logs, detection methods, and threat intelligence. This room introduces key components of a Security Operations Center (SOC), including *SIEM*, *logs*, *alerting*, and *prevention* mechanisms.
🎯 Learn how defenders identify, analyze, and stop cyber attacks before or during incidents.
.

---

## 🔐 Core Topics Covered

| 🧩 Topic               | 🔍 Description                                                                 |
|------------------------|--------------------------------------------------------------------------------|
| 🏢 Security Operations Center (SOC) | Team that detects and responds to threats                        |
| 📄 Logs                | Records of system/application events – vital for investigations               |
| 🚨 Alerts             | Notifications triggered by suspicious behavior                                 |
| 🧠 Threat Intelligence | Knowledge about attackers, tools, and techniques                              |
| ⚔️ Detection vs Prevention | Detection = monitoring, Prevention = stopping attacks                  |

---

## 🧪 Lab Activities Overview

| 🛠️ Activity                    | 💻 What You Did                                                   |
|-------------------------------|-------------------------------------------------------------------|
| SOC Tier Analysis             | Understood Tier 1 (alert triage), Tier 2 (analysis), Tier 3 (hunting) |
| Log Analysis Basics           | Learned how to read, filter, and investigate system logs          |
| Detection Techniques          | Studied signature-based and behavioral-based detection            |
| Prevention Methods            | Firewalls, AV, Endpoint Defense, WAFs                             |
| Threat Intelligence Sources   | Explored feeds like MISP, VirusTotal, AlienVault OTX              |

---

## ⚙️ Sample Terminal/Concept Snippets

```bash
# Example: Syslog log entry format
Jan 18 10:45:12 server sshd[1010]: Failed password for invalid user root

# Example: SIEM Dashboard View
- Login attempts: 450
- Failed logins: 230
- Geo-location alerts: 5 countries

# Example: Alert Rule Logic
IF login_failures > 5 FROM same_IP WITHIN 2_minutes => Raise Alert!
