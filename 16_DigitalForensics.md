# 🧪 DIGITAL FORENSICS – TryHackMe Professional Report

🕵️ Investigate. Recover. Analyze. | 🔍 Forensics for Cyber Incidents  
✅ **Room:** Digital Forensics  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/room/digitalforensics)  
👨‍💻 **Author:** **Asibur Khan** • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

*Digital Forensics* is the art and science of investigating digital devices to uncover evidence. This TryHackMe room introduces foundational forensics skills like memory analysis, disk image inspection, file recovery, and metadata investigation — essential for any cybersecurity analyst.
🎯 Learn how professionals analyze digital evidence to solve cyber crimes and incidents.
.

---

## 📁 Core Topics Covered

| 🔍 Topic             | 📘 Description                                                                 |
|----------------------|--------------------------------------------------------------------------------|
| 💽 Disk Imaging      | Creating exact copies of storage devices for analysis                         |
| 🧠 Memory Analysis   | Investigating RAM dumps for suspicious processes or credentials               |
| 🧾 File Carving      | Recovering deleted or hidden files from raw data                              |
| 🗂️ Metadata Analysis | Analyzing file attributes like creation time, modification history            |
| 🧪 Forensic Tools     | Use of Autopsy, FTK Imager, Volatility, strings, exiftool                     |

---

## 🧪 Lab Activities Summary

| 🛠️ Activity                     | 💻 What You Did                                                    |
|-------------------------------|--------------------------------------------------------------------|
| Mount & Explore Disk Images   | Used Autopsy to navigate through file system of a disk image       |
| Carved Deleted Files          | Recovered PNG/JPGs and documents from raw unallocated space        |
| Metadata Inspection           | Used exiftool to extract timestamps and camera info from images  |
| Memory Analysis with Volatility | Detected running processes, extracted browser history & passwords |
| Keyword Search                | Used string search to identify suspicious content in memory/disk   |

---

## ⚙️ Sample Commands & Forensic Work

```bash
# Mounting disk image (Linux)
sudo mount -o loop image.dd /mnt/image

# Viewing metadata with exiftool
exiftool suspect_image.jpg

# Volatility: list processes
volatility -f memdump.raw --profile=Win10x64_18362 pslist

# Recover deleted images
photorec image.dd

# Searching for strings
strings memdump.raw | grep 'password'
