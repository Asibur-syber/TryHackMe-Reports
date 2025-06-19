# 🛡️ TryHackMe Report: SOC Level 1

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [SOC Level 1 on TryHackMe](https://tryhackme.com/room/soclevel1)

---

## 🧠 1. Room Overview

This room provides a practical introduction to the day-to-day duties of a *SOC (Security Operations Center) Level 1 Analyst*.  
It focuses on real-world log analysis, alert triaging, identifying Indicators of Compromise (IOCs), and using *SIEM tools* to detect and respond to threats.

---

## 🧪 2. Tools & Technologies Used

| Tool          | Purpose                            |
|---------------|-------------------------------------|
| *Splunk*     | Log collection & correlation        |
| *VirusTotal* | Analyze suspicious domains/files    |
| *WHOIS*      | IP/domain information lookup        |
| *SIEM Tools* | Real-time monitoring and detection  |

---

## 🚀 3. Step-by-Step Process

### 🔍 Step 1: Understand SOC Analyst Role
- Learned how a SOC team operates in layers (L1, L2, L3)
- Understood alert lifecycle from detection → escalation → response

### 🧾 Step 2: Log Analysis with Splunk
- Queried various logs (Windows Events, Firewalls, Web Access Logs)
- Detected brute-force login attempts using failed login patterns
- Correlated multiple events to detect lateral movement attempts

### 🕵️ Step 3: IOC Identification
- Used WHOIS and VirusTotal to enrich suspicious IPs/domains
- Identified phishing URLs and payload delivery mechanisms
- Tagged events as malicious, suspicious, or benign

---

## 🎯 4. Captured Flags

- ✅ User Flag: THM{S0C_L3V3L_1_FL4G}

---

## 📘 5. Key Takeaways

- 🧠 Developed real-world SOC investigation skills  
- 📊 Learned how to work with SIEM dashboards and filters  
- 🕵️ Improved ability to identify true vs. false positives  
- ⚠️ Learned how to respond to alerts based on severity and impact  

---

## 🖼️ 6. Supporting Screenshots
📌 **Splunk Dashboard Example**  
 
![Splunk Logs](splunk_dashboard.png)
📌 **Alert Analysis Example**  
 
![Alert Triage](alert_investigation.png)


---

## ✍️ 7. Personal Notes

- Always validate alerts with external threat intelligence.
- Log noise is common – filtering and prioritizing is critical.
- This room truly simulates the L1 SOC environment and prepares you for real jobs.

---

🔚 *End of Report*  
📁 GitHub Repository: [TryHackMe-Reports](https://github.com/Asibur-syber/TryHackMe-Reports)
