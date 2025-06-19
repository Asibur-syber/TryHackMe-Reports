# 🔎 TryHackMe Report: Google Dorking

*👤 Completed by:* Asibur Khan  
*📅 Date:* 19-06-2025  
*🔗 Room URL:* [Google Dorking on TryHackMe](https://tryhackme.com/room/googledorking)

---

## 🧠 1. Room Overview

This room focuses on *Google Dorking*, an advanced search technique using specific queries to find sensitive information exposed on the internet.  
It is a powerful method for reconnaissance and gathering intelligence before launching attacks.

---

## 🛠️ 2. Tools & Techniques Used

| Technique     | Description                              |
|---------------|------------------------------------------|
| Google Search | Using advanced operators for precise results |
| filetype:   | Searching specific file types             |
| intitle:    | Searching page titles                      |
| inurl:      | Searching URLs for keywords                |
| site:       | Restricting search to specific domains    |

---

## 🚀 3. Step-by-Step Exploitation Process

### Step 1: Basic Dorking
- Used queries like site:example.com and filetype:pdf to discover sensitive documents.

### Step 2: Finding Login Pages
- Queried intitle:"login" or inurl:"admin" to locate possible admin panels.

### Step 3: Extracting Sensitive Data
- Combined dorks such as filetype:xls inurl:"password" to find exposed spreadsheets with credentials.

### Step 4: Mapping Target Infrastructure
- Used site:target.com -www to identify subdomains and related assets.

---

## 🎯 4. Findings & Flags

- ✅ Discovered multiple sensitive documents and admin portals.
- ✅ Identified exposed credentials and configuration files.

---

## 📚 5. Key Learnings

- Google Dorking enhances reconnaissance by uncovering data not visible through standard browsing.
- Combining operators refines search results for specific intelligence.
- Ethical use is critical — always stay within legal boundaries.

---

## 📸 6. Supporting Screenshots
📌 **Example of Google Dork Query**  
 
![google-dork](google_dork.png)
📌 **Sensitive Document Found via Dorking**  
 
![dork-doc](dork_document.png)


---

## ✍️ 7. Personal Notes

- Regular practice sharpens the ability to craft effective dorks.
- Always verify results to avoid false positives.
- Use Google Dorking responsibly to aid ethical hacking.

---

🔚 *End of Report*  
📁 GitHub Repository: [TryHackMe-Reports](https://github.com/Asibur-syber/TryHackMe-Reports)
