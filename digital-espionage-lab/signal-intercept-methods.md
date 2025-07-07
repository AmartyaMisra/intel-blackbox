# signal-intercept-methods.md

> *“All communication is signal. All signal is interceptable.”*

---

## 📡 What is Signal Interception?

Signal interception refers to the act of capturing and analyzing **electromagnetic signals**—including voice, data, and metadata—transmitted via wireless mediums. It's the backbone of both military-grade **SIGINT (Signal Intelligence)** and covert surveillance.

Whether it's a whispered phone call, satellite ping, or data handshake—if it moves through the air, it can be intercepted.

---

## 🛰️ Categories of Signal Intercept

### 1. **Cellular Communications (2G/3G/4G/5G)**

* Voice, SMS, data
* Intercepted via rogue BTS towers, femtocells, or lawful interception

### 2. **Satellite Interception**

* Used to intercept long-range diplomatic/military comms
* Captured using large parabolic dishes

### 3. **Wi-Fi & Bluetooth**

* Short-range signals
* Targets include data packets, MACs, beacon frames

### 4. **Radio Communications (VHF/UHF/HF)**

* Intercepts police, military, aviation, maritime, ham radio

### 5. **Radar and Telemetry Signals**

* Used in aircraft tracking, missile guidance, space operations

> Any unencrypted signal is fair game in modern interception.

---

## 🛠️ Tools & Hardware

### Open Source / COTS

* **RTL-SDR**: Inexpensive USB dongle, used for basic RF capture
* **HackRF One**: Wideband SDR (1 MHz – 6 GHz), for mid-level ops
* **YateBTS**, **OpenBTS**: Software for building rogue cellular towers

### Advanced / Classified

* **IMSI Catchers / Stingrays**
* **DIRNSA systems**: Satellite interception via ground stations
* **ECHELON**, **TEMPORA**: Global passive interception networks

---

## 🎯 Techniques

### 1. **Passive Interception**

* No signal injection
* Receiver silently captures signals
* Lower risk of detection

### 2. **Active Interception (MITM)**

* Involves signal manipulation
* Fake towers, fake Wi-Fi hotspots, BLE spoofing

### 3. **Lawful Intercept (LEA Backdoors)**

* Telecom equipment has built-in lawful intercept modules (CALEA compliance)
* May be abused by insiders or hostile states

### 4. **Satellite Footprint Capture**

* Capture downlink frequencies of VSAT, C-band, Ku-band
* Often used to intercept feeds in conflict zones (e.g., Syria, Ukraine)

---

## 🧪 Notable Operations

### 🇺🇸 ECHELON

* Five Eyes-operated global signal intercept grid
* Targets everything from fax to undersea fiber signal bleed

### 🇨🇳 Great Firewall + Deep Packet Inspection

* Intercepts + alters traffic crossing borders
* Used to block or surveil encrypted comms

### 🇮🇱 Israeli Military SIGINT (Unit 8200)

* Known to intercept regional communications including satellite, mobile, radio

### 🇷🇺 SORM System

* Deep integration with Russian ISPs to capture and store all citizen communications

---

## 🔍 Detection & Countermeasures

### Against Cellular Intercepts

* Use **eSIMs** and avoid 2G
* Monitor for rogue towers (e.g., **SnoopSnitch**, **Cell Spy Catcher**)

### Against Satellite Intercepts

* Encrypt all data transmissions
* Use frequency hopping or spread spectrum

### Against RF Intercepts

* Faraday cages
* Encrypted radio systems (e.g., TETRA, P25)

> Most users have no idea their phones betray them via background signals every second.

---

## 🌍 India-Specific Context

* Government plans **Centralized Monitoring System (CMS)** to tap all mobile and landline communications
* Tactical intercept tools deployed in Naxal areas, borders
* RAW/NTRO capable of satellite and RF interception

---

## 🔚 Conclusion

In the silent war of airwaves, power belongs not to who speaks—but to who listens. From SDRs in backpacks to orbital dishes in deserts, signal interception defines the frontlines of digital espionage.

> *“Before they hack your network, they hijack your frequency.”*
