# PWD-Crypt

A minimalist, elegant, and fully offline deterministic password generator built with vanilla HTML, CSS, and JavaScript.


![PWD-Crypt Interface](https://github.com/ImmanuelBTaylor/pwd-crypt/blob/main/12-17-2025_at_14-17-19.png?raw=true)
![PWD-Crypt Interface](https://github.com/ImmanuelBTaylor/pwd-crypt/blob/main/12-17-2025_at_14-18-05.png?raw=true)

PWD-Crypt allows you to generate strong, repeatable passwords for any account by combining three custom inputs (e.g., a master password, site name, and personal identifier) with secure cryptographic hashing. The same inputs and settings will **always** produce the exact same password — perfect for password management without storing anything.

No data is sent anywhere. Everything runs locally in your browser using the Web Crypto API.

## Features

- **Fully deterministic** — identical inputs yield identical passwords
- **Secure hashing** — SHA-256 (default), SHA-384, SHA-512, or chained combinations
- **Customizable output** — choose length (12–32 characters) and character sets (lowercase, uppercase, numbers, symbols)
- **Zero dependencies** — pure vanilla JavaScript, no frameworks or external libraries
- **Offline-first** — works without internet after download
- **Privacy-focused** — nothing is logged, transmitted, or stored
- **Beautiful minimalist design** with calming earth tones

## How to Use

1. Save the provided HTML file as `pwd-crypt.html`
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge)
3. Enter your three secret inputs:
   - Input 1: e.g., your master password
   - Input 2: e.g., the website or service name (like "github.com")
   - Input 3: e.g., your username or a personal token
4. Select one or more hash methods (hold Ctrl/Cmd to select multiple for chaining)
5. Adjust length and character options as desired
6. Click **Generate Password**
7. Copy the result and paste it into your account's password field

> Tip: Use consistent patterns for inputs (e.g., always put site name in Input 2) to make recreation easy.

## Security Notes

- This tool uses cryptographically secure hashing via the browser's `crypto.subtle` API.
- Passwords are derived from hash bytes mapped to your chosen character set.
- Never share your inputs or this file with untrusted parties.
- For maximum security, use a strong and unique master input (Input 1).

## Why This Tool?

Unlike cloud-based password managers, PWD-Crypt:
- Requires no account
- Stores no passwords
- Works offline
- Gives you full control

It's ideal for those who prefer stateless, reproducible password generation similar in spirit to tools like Hash-based Password or SuperGenPass — but with a modern, polished experience.

## License

This project is open source and free to use, modify, and distribute for personal use.

No attribution required.

---

Made with care for privacy and simplicity.
