# Safe Use of Public WiFi

## **Briefing**
Public WiFi is convenient — and dangerous.  
Airports, cafés, hotels, and malls are prime hunting grounds for cybercriminals.  
When you connect without precautions, you expose your data to interception, manipulation, or outright theft.

**Key reality:** Public WiFi ≠ Secure WiFi.  
Treat it as a *hostile network* by default.

---

## **Threat Vectors**
Below are common ways attackers exploit public WiFi:

1. **Rogue Access Points (Evil Twins)**  
   - Fake hotspots mimicking legitimate networks (e.g., `Cafe_WiFi_Guest`)  
   - Controlled by attackers to intercept traffic.

2. **Man-in-the-Middle (MITM) Attacks**  
   - Attacker positions themselves between you and the internet, capturing unencrypted data.

3. **Session Hijacking**  
   - Stealing active session cookies to gain access to accounts without passwords.

4. **Traffic Sniffing**  
   - Monitoring unencrypted data packets to harvest credentials, messages, or files.

5. **Malware Injection**  
   - Compromised networks that deliver malicious payloads to connected devices.

---

## **Defensive Protocol**
Adopt the following countermeasures to minimize risk:

### **1. Use a VPN**
- Encrypts all traffic, even over insecure networks.
- Choose a provider with:
  - No logs policy
  - Kill switch feature
  - AES-256 encryption

### **2. Disable Auto-Connect**
- Turn off "Connect Automatically" in WiFi settings.
- Prevents accidental connection to malicious APs.

### **3. Limit Sharing**
- Disable file/printer sharing and AirDrop/Bluetooth when not in use.
- On Windows: Control Panel → Network and Sharing Center → Advanced sharing settings.
- On macOS: System Preferences → Sharing → Uncheck all.

### **4. Verify the Network**
- Ask staff for the exact network name and password.
- Beware of similarly named look-alike SSIDs.

### **5. Stick to HTTPS**
- Avoid websites without HTTPS.
- Install browser extensions like **HTTPS Everywhere**.

### **6. Logout After Use**
- Close accounts and browser tabs when done.
- Prevents session hijacking.

---

## **Operational Example**
**Incident:**  
In 2018, a Buenos Aires café’s public WiFi was cloned by attackers using a device smaller than a deck of cards.  
Result: Dozens of customers had banking credentials stolen within minutes.

**Lessons Learned:**  
- Users auto-connected without verifying SSID.  
- No VPN usage.  
- Victims stayed logged into email and banking apps.  

**Prevention:**  
- A 30-second verification of SSID + VPN could have stopped the breach entirely.

---

## **Quick Checklist Before Connecting**
✅ VPN ON  
✅ Auto-connect OFF  
✅ Sharing OFF  
✅ HTTPS ONLY  
✅ Logout after use  

---

**Final Takeaway:**  
Public WiFi is like walking through a warzone without body armor.  
Either protect yourself — or expect to be a casualty.
