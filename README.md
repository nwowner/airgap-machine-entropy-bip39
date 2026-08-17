# ⚡ nwowner- airgap-machine-entropy-bip39

CSPRNG goes brrr. 🚫🔌 `window.crypto` pulls raw machine entropy directly from your local hardware—not predictable math.

The ultimate alternate-history BIP-39 key generator by **nwowner** (the name that *should* have been on the whitepaper but would have never been taken seriously). 

This is a zero-dependency, single-file HTML application built for maximum privacy, sovereign self-custody, and true air-gapped execution. It maps 128/256 bits of hardware-harvested entropy into cryptographically secure 12 or 24-word seed phrases following the exact Bitcoin BIP-39 protocol standard.

---

## 🔒 Security Architecture

1. **Hardware-Driven Randomness:** Uses native `window.crypto.getRandomValues()` to harvest entropy directly from your system's hardware state. It layers this with a real-time mouse-movement pooling mechanism to inject additional chaotic machine entropy.
2. **Zero Network Exposure:** No external CDNs. No Google Analytics. No third-party Javascript packages. Everything—from CSS layouts to the cryptographic hashing engine—is self-contained in a single file.
3. **Environment Threat Monitor:** Built-in proactive scanning that inspects network status, checks window dimensions for malicious background mirroring/recording, monitors script load origins, and warns you if the browser detects a non-air-gapped environment.

---

## 🚀 How to Execute Like a Sovereign Pleb

While this tool can be hosted on GitHub Pages for distribution convenience, **NEVER generate production keys on a machine actively connected to the internet.** 

Follow the proper air-gap protocol:

1. **Download:** Save the `index.html` file from this repository onto a clean, empty USB flash drive.
2. **Isolate:** Boot an isolated computer, prefer using an ephemeral live operating system (like Tails OS or a fresh Ubuntu live USB). 
3. **Disconnect:** Physically pull out your Wi-Fi cards, disconnect Ethernet cables, and turn off Bluetooth.
4. **Run:** Insert your USB drive, open the local `index.html` file inside an open-source browser (Firefox/Chromium), pass the Environment Checks, and generate your keys.
5. **Secure:** Physically write your words down on paper or stamp them into steel. Do not take photos or save screenshots. Back in the day I used a Polaroid camera, but those are probably extinct now. 

---

## 🛠️ Verification & Math

The internal SHA-256 integrity check allows you to verify that the code running in your browser matches the raw cryptographic hash of the source code file. 

* **Protocol Alignment:** BIP-0039 standard compliant
* **Entropy Engine:** CSPRNG + Mouse Hardware Seed Mixer
* **KDF / Hashing Layer:** Native Web Cryptography API (`SubtleCrypto`)

*Made by NWOwner. Your hardware, your sovereign wealth.*

