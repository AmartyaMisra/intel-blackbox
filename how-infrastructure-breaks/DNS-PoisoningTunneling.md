# DNS Poisoning & Tunneling: Hijacking the Internet’s Address Book

> *“If the internet is a city, DNS is its map. Poison the map, and you mislead the world.”*

---

## 🌐 What is DNS?

**Domain Name System (DNS)** is the internet’s address book. It translates human-friendly URLs like `example.com` into machine-readable IP addresses like `93.184.216.34`.

Without DNS, we’d need to memorize raw IPs to visit websites.

---

## 🧠 DNS Workflow (Simplified)

1. You type `google.com`
2. Browser asks your **local DNS resolver**
3. Resolver queries **root DNS**, then **TLD (.com)**, then **authoritative server**
4. IP is returned → connection made

All this happens in milliseconds. But it’s exploitable.

---

## ☠️ What is DNS Poisoning (aka DNS Spoofing)?

**DNS poisoning** is when an attacker injects false DNS responses into the lookup process. Your browser gets the wrong IP and connects to a fake or malicious site.

> You think you're logging into `bank.com`, but it’s a phishing mirror.

---

## 💣 Attack Vectors

### 1. **Man-in-the-Middle (MitM)**

* Attacker intercepts DNS requests on public Wi-Fi
* Sends fake reply before real server can

### 2. **Cache Poisoning**

* Poison recursive resolvers with bad entries
* Affects everyone who uses that resolver

### 3. **Compromised Authoritative DNS**

* Hacker gains access to domain registrar or DNS host
* Changes records directly (e.g., `A`, `CNAME` entries)

### 4. **BGP Hijacking + DNS Poisoning**

* Hijack internet routes to redirect DNS traffic through malicious infrastructure

---

## 🔍 Real Incidents

* **China's Great Firewall**: Injects poisoned DNS for `facebook.com`, `nytimes.com`
* **ComodoHacker (2011)**: Used DNS to redirect users to fake SSL cert providers
* **MyEtherWallet DNS Hijack (2018)**: \$150k stolen via poisoned DNS to phishing server

---

## 🕳️ What is DNS Tunneling?

**DNS tunneling** hides data inside DNS queries and responses. Used for:

* **Data exfiltration** from locked-down networks
* **Backdoors** and command-and-control (C2) channels
* **Bypassing firewalls** in restricted environments

### How It Works:

* Encode data in subdomain of DNS query (e.g., `secret-data.attacker.com`)
* Attacker’s DNS server decodes payloads

> Looks like normal DNS traffic. But it’s smuggling secrets.

---

## 🧪 Tools Used

* `dnscat2`: Tunnels shell access via DNS
* `iodine`, `dns2tcp`: Data transfer tools over DNS
* Metasploit modules for DNS backdoors

---

## 🛡️ Detection & Defense

### For Poisoning:

* Use **DNSSEC** (DNS Security Extensions)
* Pin trusted DNS (Cloudflare `1.1.1.1`, Google `8.8.8.8`)
* Enforce **DoH/DoT** (DNS over HTTPS / TLS)

### For Tunneling:

* Analyze **query volume & entropy**
* Flag **long subdomains** or frequent failed lookups
* Use **AI/ML threat models** to flag covert channels

> Normal DNS looks like street signs. Tunneling looks like encrypted graffiti.

---

## 🌍 India-Specific Context

* State-level censorship sometimes involves **forced DNS poisoning**
* Many users rely on **ISP DNS**, vulnerable to MitM
* Mass-level filtering in Kashmir, Assam, etc., often uses DNS layer

---

## 🔚 Conclusion

DNS is fragile and fundamentally trust-based. Its manipulation is quiet, powerful, and often invisible to the average user. Poison it—and you don’t break the internet. You **redirect it**.

> *“The pen may be mightier than the sword. But DNS is mightier than both.”*
