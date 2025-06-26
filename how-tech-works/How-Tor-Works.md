# How Tor Works: The Architecture of Anonymity

> *“Tor doesn’t make you invisible. It makes you anonymous—until you reveal yourself.”*

---

## 🎯 What is Tor?

**Tor (The Onion Router)** is a network designed to enable **anonymous communication** across the internet by encrypting and routing traffic through multiple servers (called nodes or relays). It was initially developed by the **U.S. Naval Research Lab** for intelligence communications and is now an open-source project used by journalists, whistleblowers, activists—and yes, cybercriminals.

---

## 🧠 Core Concepts

### 🔁 Onion Routing

* Your data is **wrapped in layers of encryption**—like an onion
* Each node decrypts **only its own layer**, revealing the next destination
* No single node knows both the source and final destination

### 🧩 The Tor Network

* Thousands of **volunteer-run servers** (nodes) around the world
* Composed of:

  * **Guard Node**: Your entry point into Tor
  * **Middle Relay**: Passes encrypted data deeper into the network
  * **Exit Node**: Final node that decrypts and forwards your data to the internet

---

## 🔄 Step-by-Step: How Tor Sends Your Data

1. **Tor client** chooses 3 relays at random: Guard → Middle → Exit
2. Your message is **triple-encrypted** (for each relay)
3. Message passes through:

   * Guard decrypts 1st layer ➝ forwards
   * Middle decrypts 2nd ➝ forwards
   * Exit decrypts final layer ➝ sends to destination
4. Server response follows the same path **in reverse** (re-encrypted at each layer)

> Your ISP sees only that you're connected to a Guard Node—not what you're doing.

---

## 🔒 Encryption Used

* Uses **TLS-like protocols** for outer shell
* Each hop re-encrypts data using **public/private key pairs**
* Ensures **perfect forward secrecy**: session keys can’t decrypt past logs

---

## 🌐 .onion Sites: Tor’s Hidden Services

Tor can also host websites—called **hidden services**—with domains ending in `.onion`. These aren’t accessible via normal browsers.

How it works:

* Site generates public key ➝ forms a .onion address
* Advertises itself to Tor network via **Introduction Points**
* Clients connect via **Rendezvous Points** without ever revealing IPs

> Examples: ProtonMail’s Tor mirror, SecureDrop for whistleblowers, and dark web marketplaces.

---

## 🧪 Real-World Use Cases

* **Journalists** communicating securely with sources
* **Citizens** in censored regimes (China, Iran)
* **Dark web commerce** (drugs, data dumps, hacking services)
* **Malware C2 Servers** hiding their backend infrastructure

---

## 🕳️ Limitations & Vulnerabilities

* **Exit Nodes are not encrypted** ➝ They can see plain data if site isn’t HTTPS
* **Traffic correlation attacks** by powerful adversaries (e.g., NSA)
* **JavaScript/Browser leaks** can de-anonymize users
* **Timing attacks**: match when data enters & exits the network
* Some nodes may be **malicious or government-run**

> Tor is not a magic cloak. One bad browser plugin can betray you.

---

## 🛡️ How to Use Tor Safely

* Use **Tor Browser only** (do not use Chrome + proxy)
* Disable JavaScript and browser plugins
* Don’t login to real identity accounts (Gmail, Facebook)
* Avoid downloading files (PDFs can beacon your IP)
* Never go full-screen (screen size fingerprinting risk)

---

## 🔚 Conclusion

Tor is a masterpiece of **decentralized anonymity**, but it’s not foolproof. It protects your identity only if you **don’t betray yourself**. Understand its architecture, respect its limits, and use it for what it was built for: **privacy in a surveillance-heavy world**.

> *"Tor hides the road, but not the footprints you leave behind."*
