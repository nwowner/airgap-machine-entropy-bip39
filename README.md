# ⚡ nwowner-genesis // Sovereignty Engine

> "CSPRNG goes brrr. 🚫🔌 `window.crypto` pulls raw machine entropy directly from your local hardware—not predictable math."

The ultimate alternate-history BIP-39 key generator by **nwowner** (the name that *should* have been on the Bitcoin Whitepaper). 

This is a zero-dependency, single-file HTML application built for maximum privacy, anti-keylogger protection, and true air-gapped execution. It maps 128/256 bits of hardware-harvested machine entropy into cryptographically secure 12 or 24-word seed phrases following the exact Bitcoin BIP-39 protocol standard.

---

## 🔒 Advanced Security Architecture

1. **Expanded Sandbox Coordinate Area:** The entropy-harvesting playground features an expanded 280px canvas container. Sweeping your mouse inside this grid injects high-resolution human micro-movement timing noise over the machine's underlying CSPRNG hooks.
2. **Anti-Keylogger Matrix Keyboard:** Includes a randomized virtual input engine utilizing a Fisher-Yates shuffle algorithm. Keys scramble dynamically on every single click, entirely bypassing hardware or software keyloggers monitoring your operating system keyboard input layout.
3. **BIP-39 Passphrase Support:** Full deployment for the optional "25th word" passphrase layer, creating a hidden, custom wallet matrix side-by-side with your standard seed phrase.

---

## 🛠️ The Cryptographic Telemetry Drawer: Verified Offline

In Bitcoin, the motto is **"Don't Trust, Verify."** These four live-rendered cryptographic parameters serve as your local proof of mathematical honesty.

### 🧬 1. Local Machine Hardware Entropy (XOR Layered Hex)
* **What it is:** A direct window into your machine's physical hardware state combined with your unique mouse movement timing pixels.
* **Why it matters:** If this hex ever looks identical or follows a predictable pattern when refreshing, the system is rigged. It must be mathematically unique every time.

### 🔑 2. Derived 512-bit Root Seed Hex (BIP-39 Pbkdf2 Signature)
* **What it is:** The mathematical master key stretching your written English words and your passphrase together using a local PBKDF2-SHA512 hashing layer.
* **Why it matters:** This proves your local code executed the exact protocol standard. You can test your words in an independent offline calculator (like Ian Coleman's tool) and it will render this identical master hex.

### 🏴 3. Master Private Key (`xprv`) & Watch-Only Public Key (`xpub`)
* **What it is:** The Hierarchical Deterministic (HD) root key strings used to derive all subsequent Bitcoin addresses and child keys.
* **Why it matters:** These strings are fully unlocked using an embedded, standalone cryptographic calculation script. They display instantly on **any device or web browser**, even when opened as a completely isolated raw local file (`file://`) with zero internet.

---

## 🚀 How to Execute Like a Sovereign Pleb

Never generate production-grade keys while actively connected to the internet. Follow the proper air-gap protocol:

1. **Download:** Save your single `index.html` file onto a clean, empty USB flash drive.
2. **Isolate:** Boot an isolated computer using an ephemeral live operating system (like Tails OS). 
3. **Disconnect:** Physically pull out your Wi-Fi cards, disconnect Ethernet cables, and turn off all network interfaces entirely.
4. **Run:** Open the local `index.html` file inside an open-source browser, fill the entropy canvas, select your passphrase variables, and generate your keys.
5. **Secure:** Physically write your words down on paper or stamp them into steel. Do not take photos, screenshots, or cloud backups.

---

## 📲 How to Use Your Generated Wallet

Your generator creates a standard, universally recognized **BIP-39 mnemonic phrase**. To load it into an everyday device:

* **Hardware Wallets (Recommended):** Open your device (Jade, Coldcard, BitBox02, Trezor), select "Import/Restore Wallet", and enter your 12/24 words.
* **Mobile/Desktop Wallets:** Load open-source software (BlueWallet, Electrum, Sparrow), select "Import from Seed", and type your phrase.
* **Crucial Setting:** If you enabled the optional **25th-word passphrase** in your generator, you must toggle "Passphrase support" or "BIP-39 Passphrase" in your wallet software and type it in there, or you will open a completely different, empty wallet profile.

*Made by nwowner. Your hardware, your sovereign wealth.*
