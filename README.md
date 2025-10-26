# Simple Passphrase Generator

> Generate secure, human-readable passphrases — **color + object + integer** — designed for phone-friendly, temporary logins.  
> Live app: [https://martinvicknair.github.io/simple-passphrase-generator/](https://martinvicknair.github.io/simple-passphrase-generator/)

---

## ✳️ Overview

The Simple Passphrase Generator builds short but strong passphrases using a simple readable pattern:

> **color + object + integer**

Examples:
blue-wolf-823 
green.cactus.4832 
orange-horse-213 

Each phrase:
- Uses a **random color** followed by one or more random **objects** (animals, vegetables, or minerals)
- Appends a **3- or 4-digit integer** (no leading zero)
- Chooses one consistent separator (`.` or `-`) per passphrase
- Meets or slightly exceeds a user-set **minimum total length**

---

## 🧠 Why It Exists

Typical password generators output unreadable strings (`Xq8$L0!`), which are impractical for over-the-phone resets or short-term access codes.  
This tool balances **security** and **readability**:

- **Easy to pronounce** and confirm verbally  
- **Memorable enough** for short sessions  
- **Cryptographically random** (via Web Crypto API)  
- **Client-side only** – nothing is sent or logged  

---

## 🔐 Entropy & Combinations

At the minimum 12-character setting:

| Parameter | Value |
|------------|-------|
| Possible combinations | **≈ 1.47 million** |
| Approximate entropy | **≈ 20.5 bits** |
| Digits used | 3 – 4 digits (first 1–9) |
| Word sources | 10 colors + 80 objects |
| Separators | `.` or `-` |

Longer minimums increase entropy proportionally.

---

## ⚙️ Features

- Adjustable **minimum length** (12 – 20 chars)  
- Fully **offline** — runs 100 % in your browser  
- Copy-to-clipboard with visual feedback  
- Randomly chosen consistent separator per phrase  
- No leading zeros and filters banned numbers  
- **Accessible:** keyboard-friendly, ARIA labels, high-contrast dark theme  

---

## 🧩 Tech & Implementation

- **HTML5 + Vanilla JS** only  
- **Web Crypto API** for randomness  
- **Static single-page app** hosted on GitHub Pages  
- Inlined CSS for instant load  

---

## 🧱 Structure
simple-passphrase-generator/
├── index.html # App UI and generator logic
├── favicon.png # Optional browser icon
├── og-preview.png # Social preview image
├── sitemap.xml # SEO sitemap
├── robots.txt # Crawl directives
└── LICENSE # CC BY 4.0 license

---

## 🚀 Deployment

This is a **one-page static app** — simply upload `index.html` (and optional image/icon files) to any web server or host it with **GitHub Pages**.

- To rename or rebrand, edit the `<title>` and meta tags in the `<head>`.  
- No build tools, database, or dependencies required.

---

## 🔍 SEO & Discoverability

Optimized with:
- Canonical URL + meta description + keywords  
- Open Graph & Twitter cards  
- Schema.org `WebApplication` markup  
- Sitemap + robots.txt  
- Crawlable text section for keywords  

---

## 🧑‍💻 Contributing

Fork and modify freely:
- Word lists in the **“Editable Constants”** section of `index.html`  
- Banned substrings or numbers  
- Default minimum length or UI text  

Pull requests for UI, accessibility, or language support are welcome.

---

## 📜 License

**Creative Commons Attribution 4.0 International (CC BY 4.0)**  
© 2025 [Martin Vicknair](https://github.com/martinvicknair)

If you reuse or adapt this project, please credit:

> *“Based on Simple Passphrase Generator by Martin Vicknair (CC BY 4.0)”*

---

## 📸 Preview

![Simple Passphrase Generator Screenshot](og-preview.png)

---

### 🔑 Keywords

`passphrase generator`, `secure password generator`, `memorable passphrase`,  
`temporary login password`, `CSR support`, `phone verification`,  
`offline password tool`, `Web Crypto API`, `secure temporary passwords`

---

**Live app:** [https://martinvicknair.github.io/simple-passphrase-generator/](https://martinvicknair.github.io/simple-passphrase-generator/)

