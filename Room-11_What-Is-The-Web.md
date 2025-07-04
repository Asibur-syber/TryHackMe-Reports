# 🧑💻 ASIBUR RAHAMAN  
**Ethical Hacker | Web Recon Specialist | Burp Suite Explorer**  
🔗 GitHub: [github.com/Asibur-syber](https://github.com/Asibur-syber)

---

# 🌐 TRYHACKME ROOM REPORT — 11: WHAT IS THE WEB  
🔗 [Room Link → https://tryhackme.com/room/whatisweb](https://tryhackme.com/room/whatisweb)

---

## 🧠 EXECUTIVE SUMMARY

This room serves as a **foundational gateway into web hacking** by explaining how the World Wide Web functions at its core. It dissects key web components — including **HTTP/HTTPS**, **DNS**, **Web Servers**, **URLs**, and **frontend technologies (HTML/CSS/JS)**. Understanding these components is **non-negotiable** for aspiring ethical hackers looking to exploit web-based vulnerabilities like XSS, SQL Injection, and CSRF.

---

## 🧭 STEP-BY-STEP LEARNING BREAKDOWN

### 🔹 Task 1: What is the Web?
- The **internet** is a global system of interconnected networks.
- The **World Wide Web (WWW)** is a service that runs on top of the internet, delivering content.
- Users access web content via **browsers** (clients), which connect to **web servers**.

### 🔹 Task 2: Hosting & Web Servers
- Websites are hosted on **web servers** like Apache, Nginx, or IIS.
- Pages are often built using **HTML**, **CSS**, and **JavaScript**.
- A **domain name** points to the server IP via **DNS resolution**.

### 🔹 Task 3: HTTP vs HTTPS
- **HTTP** (HyperText Transfer Protocol): Transmits data in plaintext.
- **HTTPS**: Secure version of HTTP using **TLS encryption**.
- HTTP Methods:
  - `GET`: Retrieve resources  
  - `POST`: Submit form data  
  - `PUT`, `DELETE`: Modify or remove data

### 🔹 Task 4: URL Anatomy
- Example: `https://www.example.com:443/index.html`
  - `https` → Protocol  
  - `www.example.com` → Domain  
  - `443` → Port  
  - `/index.html` → Resource path

### 🔹 Task 5: Domain Name System (DNS)
- **DNS** translates human-readable domains into IP addresses.
- Key Records:
  - `A`: Maps domain to IP address  
  - `CNAME`: Alias for another domain  
  - `MX`: Mail exchange records  
- Tools: `nslookup`, `dig`, `host`

### 🔹 Task 6: Web Page Components
- Websites are constructed with:
  - **HTML** → Content structure  
  - **CSS** → Styling & layout  
  - **JavaScript** → Dynamic interaction
- Browsers render these components into visual pages.

### 🔹 Task 7: Summary Quiz
- Multiple-choice and fill-in-the-blank to reinforce concepts:
  - Protocols  
  - URL anatomy  
  - DNS records  
  - Web components

---

## 🛠️ TOOLS & CONCEPTS INTRODUCED

| 🔧 Tool / Concept     | 📌 Description                          |
|----------------------|------------------------------------------|
| HTTP/HTTPS           | Core web communication protocols         |
| DNS                  | Resolves domain names to IPs             |
| Web Servers          | Hosts and serves website content         |
| URL Structure        | Accesses specific content on the web     |
| HTML/CSS/JS          | Build and design frontend user interfaces|
| Web Browsers         | Render and display web content           |

---

## 💡 PRACTICAL EXAMPLES

### ✅ Example 1: Accessing a Website
1. User enters `https://tryhackme.com`
2. DNS query resolves to server IP.
3. Browser sends an HTTPS request.
4. Server returns an HTML response.
5. Browser renders page with CSS/JS.

### ✅ Example 2: DNS Lookup
- Command: `nslookup tryhackme.com`  
  → Shows the IP address of the domain.

### ✅ Example 3: Viewing Web Source
- Press `Ctrl + U` in browser  
  → Reveals raw HTML/CSS code behind the page.

---

## 📸 RECOMMENDED SCREENSHOTS

| 🖼️ Screenshot Filename        | 🔍 Purpose                                      |
|------------------------------|-------------------------------------------------|
| `web-dns-lookup.png`         | Output of `nslookup tryhackme.com`             |
| `http-request-header.png`    | Display of HTTP GET request headers             |
| `url-breakdown.png`          | Annotated parts of a sample URL                 |
| `dns-dig-host.png`           | DNS info using `dig` and `host`                |
| `html-css-source.png`        | Screenshot of raw HTML/CSS from browser view   |
| `network-traffic-analysis.png` | Request/Response view via browser DevTools    |

---

## 🛡️ SECURITY INSIGHTS

- A hacker must **understand how browsers communicate with servers** to intercept and manipulate traffic.
- Many vulnerabilities rely on:
  - Understanding **HTTP headers**
  - Manipulating **forms and requests**
  - Exploiting **poor JavaScript implementations**
  - Abusing **DNS spoofing** or **subdomain takeovers**
- These basics are directly tied to OWASP Top 10 vulnerabilities.

---

## 🧩 FINAL THOUGHTS

This room is **not optional** — it is the blueprint for everything to come in web exploitation. By grasping the structure and logic of web traffic, ethical hackers unlock the power to perform advanced attacks like XSS, CSRF, and SQL Injection. **Mastering the web layer is the key to mastering web hacking.**

---

## 🚀 NEXT STEPS

✅ Practice using `nslookup`, `dig`, `host` for DNS enumeration  
✅ Learn to inspect and modify HTTP traffic using **Burp Suite**  
✅ Analyze HTML source and forms manually  
✅ Move forward to [Room 12: How Websites Work](https://tryhackme.com/room/howwebsiteswork)

---

> 🌐 *“The web is not magic — it’s logic in action. Know the web, and you control the gateway.”*  
> — **ASIBUR RAHAMAN**
