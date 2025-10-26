# Simple Passphrase Generator

**Live app:** https://martinvicknair.github.io/simple-passphrase-generator/  
**Source HTML (main branch):** `simple-password-generator.html`

Generate **NIST-compliant**, human-readable passphrases that are easy to say over the phone — perfect for **temporary account resets** used by customer support reps.

> Pattern: **color + object + integer**  
> Examples: `Blue-horse-823`, `Green.cactus.4821`

---

## ✳️ Highlights

- **Readable & phone-friendly:** simple words + punctuation + digits
- **Meets most policies:** uppercase + lowercase + digits + `.`/`-` punctuation
- **Configurable length:** dropdown **12–20** (default **15**)
- **Crypto-random:** uses the browser’s **Web Crypto API**
- **Client-side only:** runs entirely in the browser — **no data is sent**
- **Copy to clipboard:** click any generated phrase (visual confirmation)
- **Accessible UI:** keyboard support, ARIA roles, high contrast
- **Customizable word lists:** edit arrays in the source

---

## 🔐 Policy & Security Notes

- First word is **always capitalized** (e.g., `Blue-…`) for clarity and to satisfy common “has uppercase” rules.
- Punctuation is `.` or `-` (chosen per phrase), typically counted as **special characters** in modern policies.
- A **3–4 digit integer** (no leading zero) is appended.
- A conservative “Over **X** unique phrases at **N+** chars” estimate is shown and updates with the **Minimum characters** selection.

> This tool is designed for **temporary password resets** and short-term access — not as a long-term master password manager.

---

## 🧩 How It Works

- Start with `Color + Object`
- Choose one separator for the whole phrase: `.` or `-`
- Add **3** digits; if the **Minimum characters** requirement isn’t met, use **4** digits; if still short, add another **Object**
- Filter phrases containing banned substrings or banned numbers (customizable)

---

🔧 Customize

Open simple-password-generator.html and edit:

Word lists (arrays at the top): COLOR, ANIMALS, VEGETABLES, MINERALS

Banned substrings / numbers: BANNED_SUBSTRINGS, BANNED_NUMS

Default minimum characters: set the <select> default option

---

🧪 Local Usage

Just open simple-password-generator.html in a modern browser. No build tools needed.

---

🔌 Zendesk App (coming soon)

This generator is being adapted as a Zendesk app for the ticket sidebar, with one-click copy or append to comment actions.

---

🏷️ GitHub Topics

passphrase-generator, secure-password, memorable-password, csr-tools, web-crypto, password-generator, security-tools, vanilla-js, github-pages, offline-tools

---

📜 License

Creative Commons Attribution 4.0 International (CC BY 4.0)  
© 2025 Martin Vicknair — You may share and adapt, including commercial use, with attribution.  
Full text: https://creativecommons.org/licenses/by/4.0/

If you reuse or adapt this project, please credit:

“Based on Simple Passphrase Generator by Martin Vicknair (CC BY 4.0)”
