# GPS Spoofing: Hacking Location in a Satellite-Led World

> *“When your map lies to you, it’s not lost—it’s hijacked.”*

---

## 📡 What is GPS?

The **Global Positioning System (GPS)** is a constellation of satellites maintained by the U.S. military that enables receivers (your phone, car, drone) to determine their position via signals from space. GPS uses **time-of-flight** measurements from at least 4 satellites to triangulate accurate location data.

Other systems: GLONASS (Russia), Galileo (EU), BeiDou (China), NavIC (India).

---

## 🧨 What is GPS Spoofing?

**GPS Spoofing** is the act of broadcasting **false GPS signals** to deceive a receiver into computing an incorrect position or time.

Unlike jamming (which blocks signals), spoofing **tricks the device**—often without any obvious disruption.

> It's not “signal noise.” It’s signal **deception**.

---

## 🔁 How Spoofing Works

1. Attacker transmits fake GPS signals mimicking real satellite data
2. Signal strength is slightly higher than real satellites
3. Target device locks onto spoofed signal
4. Location/time shifts based on attacker’s intent

Attackers may:

* Drift location slowly (undetectable)
* Jump to entirely false location (teleportation)
* Desync timing signals (to break crypto, ATM sync, etc.)

---

## 🛠️ Tools Used

* **Software-defined radios (SDRs)**: e.g., HackRF, BladeRF
* **GNSS-SDR & GPS-SDR-SIM**: Open-source spoofing frameworks
* **Replay devices**: Record and rebroadcast GPS signals

> Spoofing kits cost < \$500 but can disrupt ships, drones, and finance.

---

## 🧪 Real-World Incidents

* **Black Sea (2017)**: 20 ships reported location errors; believed to be Russian spoofing
* **Iran vs. U.S. RQ-170 Drone (2011)**: Iran claimed to spoof and capture a stealth UAV
* **China (2021)**: Ships near Shanghai showed them inland—spoofing to protect naval drills
* **Texas & NY Airports (2022)**: Aircraft experienced signal interference—possibly accidental spoof/jam

---

## 🚁 Targets of Spoofing

* **Military drones**: Misguiding flight paths
* **Shipping vessels**: Redirecting or masking location
* **Autonomous cars**: Feeding fake nav inputs
* **Crypto systems**: Break time-dependent blockchain features
* **Stock markets & data centers**: Timestamps used for trading and sync

> GPS is a silent backbone of modern systems—not just maps.

---

## 🛡️ Detection & Defense

### Technical Defenses:

* **Multi-GNSS receivers** (compare GPS, GLONASS, etc.)
* **Angle of Arrival** (AoA) detection via antenna arrays
* **Clock drift analysis**
* **Signal strength anomaly detection**

### Practical Defenses:

* Use **inertial sensors** to compare expected movement
* Implement **geofencing alerts**
* Monitor for **GPS time errors**—not just location

> GPS signals are weak; defense needs both hardware and software layers.

---

## 🇮🇳 India’s Role

* India operates **NavIC** (Navigation with Indian Constellation)
* DRDO is developing **anti-spoof GNSS receivers**
* Use in:

  * Missile guidance
  * Disaster relief
  * Railway tracking

---

## 🧠 Why It Matters

Spoofing turns navigation into misinformation. A hijacked location isn’t just a prank—it can mean misdelivered aid, grounded aircraft, lost drones, or falsified evidence.

> *“In the age of digital truth, GPS spoofing is location-level gaslighting.”*

---

## 🔚 Conclusion

GPS spoofing is no longer military-grade sci-fi—it’s field-tested, commercially accessible, and geopolitically strategic. As our infrastructure leans more on satellite signals, the threat surface rises.

> Treat your GPS signal like an open whisper in a crowded room—anyone can speak louder and lie.
