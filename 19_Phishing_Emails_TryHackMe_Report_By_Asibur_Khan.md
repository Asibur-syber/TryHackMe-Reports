# 📧 TryHackMe Report: Phishing Emails

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [Phishing Emails on TryHackMe](https://tryhackme.com/room/phishingemails)

---

## 🧠 1. Room Overview

This room focuses on understanding and identifying *phishing emails*, a major threat vector used in social engineering attacks.  
It teaches how to analyze suspicious emails, extract IOCs (Indicators of Compromise), and safely examine malicious content for threat intelligence.

---

## 🧪 2. Tools & Resources Used

| Tool / Resource   | Purpose                                 |
|-------------------|------------------------------------------|
| *Email Headers*  | Analyze sender info & email origin       |
| *VirusTotal*     | Scan links and attachments               |
| *WHOIS / IP Lookup* | Identify suspicious IPs or domains     |
| *CyberChef*      | Decode/Deobfuscate email content         |
| *Base64 Decoder* | Analyze encoded phishing payloads        |

---

## 🚀 3. Step-by-Step Process

### 🕵️ Step 1: Email Header Analysis
- Parsed raw email headers to identify sender's IP and domain.
- Verified From, Reply-To, and Return-Path fields.
- Detected spoofed sender domain not matching actual IP origin.

### 🔗 Step 2: URL and Attachment Analysis
- Extracted suspicious link from email body.
- Checked the link in VirusTotal → marked as phishing domain.
- Analyzed file attachment → detected obfuscated JavaScript payload.

### 🧪 Step 3: IOC Extraction
- Extracted the following IOCs:
  - Malicious IP: 103.29.67.12
  - Phishing Domain: secure-update-login[.]net
  - File hash (SHA256): af7db...de9a3c2

### 🔒 Step 4: Reporting and Mitigation
- Marked email as phishing and flagged it within SIEM.
- Shared indicators with threat intel team.
- Blacklisted sender domain and related URLs.

---

## 🎯 4. Captured Flags

- ✅ User Flag: THM{Ph1sh1ng_3ma1l_Analyz3d}

---

## 📘 5. Key Takeaways

- 🧠 Learned how to analyze phishing emails without clicking suspicious links.
- 🔍 Understood the importance of header forensics in verifying sender legitimacy.
- ⚔️ Gained confidence in identifying encoded payloads in malicious attachments.
- 📡 Improved threat detection using VirusTotal and WHOIS lookups.

---

## 🖼️ 6. Supporting Screenshots
📌 **Email Header Analysis Example**  
 
![Header Analysis](header_analysis.png)
📌 **VirusTotal Phishing Domain Detection**  
 
![VT Result](virustotal_phishing.png)


---

## ✍️ 7. Personal Notes

- Always treat unknown emails with caution, even if they look legitimate.
- Most phishing attempts use urgency ("Your account will be deactivated!") — recognize the pattern.
- CyberChef is extremely useful for decoding obfuscated scripts and payloads.

---

🔚 *End of Report*  
📁 GitHub Repository: [TryHackMe-Reports](https://github.com/Asibur-syber/TryHackMe-Reports)
