# 🔐 ENCRYPTION – TryHackMe Professional Report

🧠 Learn. 🔍 Practice. 💻 Hack.  
✅ **Room:** Encryption  
🌐 **Platform:** [TryHackMe.com](https://tryhackme.com/)  
👨‍💻 **Author:** Asibur Khan • [GitHub: Asibur-syber](https://github.com/Asibur-syber)  
  
📅 **Date:** June 18, 2025
5

---

## 🌟 Executive Summary

Encryption is the backbone of *digital security*. This TryHackMe room dives deep into encryption techniques, encoding, hashing, and real-world cryptographic tools. The skills practiced in this room are foundational for penetration testers, forensic analysts, and security engineers.

✅ **Mission:** Learn to lock and unlock secrets like a real ethical hacker!


---

## 📚 Topics Covered

| 🔸 Concept                  | 🔍 Description                                              |
|----------------------------|-------------------------------------------------------------|
| 🔐 Encryption               | Convert data into unreadable ciphertext                    |
| 🔁 Symmetric vs Asymmetric | Single-key (AES) vs Key-pair (RSA) encryption              |
| 🔤 Base Encodings           | Base64, Base32, Hex – for data representation              |
| 💣 Cipher Techniques        | Caesar, ROT13, XOR                                         |
| 🧱 Hash Functions           | MD5, SHA1, SHA256 – One-way fingerprinting                |
| 🛠️ Practical Tools          | CyberChef, OpenSSL, Hash-Identifier, CrackStation         |

---

## 🛠️ Hands-On Tools Used

| ⚙️ Tool           | 📌 Purpose                                 |
|------------------|---------------------------------------------|
| *CyberChef*     | Visual tool for decoding, XOR, ROT13        |
| *OpenSSL*       | Command-line encryption with AES            |
| **Hash-Identifier**| Detect hash types like MD5/SHA1/SHA256     |
| *CrackStation*  | Online hash cracker                         |
| *base64 / xxd*  | Encode/decode data from terminal            |

---

## 🔑 Key Concepts Explained

### 🟩 Symmetric Encryption
- *Same key* used to both encrypt and decrypt.
- Examples: *AES*, *DES*
- ✅ Fast, used in file encryption

### 🟦 Asymmetric Encryption
- Uses *Public key* to encrypt, *Private key* to decrypt.
- Examples: *RSA*, *ECC*
- ✅ Ideal for secure key exchange

### 🟨 Hashing
- One-way conversion of data → *Digital fingerprint*
- Used for password storage, file integrity
- Examples: *MD5*
*SHA256**

---

## 🧪 Lab Activities

### 1️⃣ Base64 Encoding/Decoding
```bash
echo "Asibur" | base64          # Encodes to: QXNpYnVy
echo "QXNpYnVy" | base64 -d    # Decodes to: Asibur
