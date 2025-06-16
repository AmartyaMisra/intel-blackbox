# OSINT vs Victim X: Anatomy of a Digital Hunt

---

## 🎯 Objective

Demonstrate how open-source intelligence (OSINT) can be used to **profile, track, and potentially compromise** a human target using only public data — no hacking required.

This is not a hack. This is **legal, lethal, and open**.

---

## 🧍‍♂️ Profile: Victim X

- Name: **Karan Sharma** (common Indian alias)
- City: Pune, India
- Occupation: Software Engineer
- Social Media: Instagram, LinkedIn, GitHub
- Email: karansharma786@gmail.com (found in pastebin leak)
- Phone: Leaked in Zomato 2019 breach

---

## 📡 OSINT Phases

### 🥇 Phase 1: Passive Recon

- **Instagram** photos reveal:
  - License plate of car
  - Apartment complex name via geo-tags
  - Gym location (based on mirror shots)
  - Frequent tagging of Starbucks Koregaon Park

- **LinkedIn** reveals:
  - Company: Infosys
  - Department: DevSecOps
  - Projects: Uses Azure, Terraform, GitLab CI

- **GitHub** handle reused from Instagram bio:
  - Repo with email in commit logs
  - AWS keys accidentally exposed in an old repo, later deleted (still indexed by Wayback Machine)

---

### 🥈 Phase 2: Behavioral Mapping

- Weekly gym check-ins: Mon/Wed/Fri mornings
- Netflix activity synced to Twitter via IFTTT
- Tweets reveal he's a fan of *Attack on Titan*, uses public transport often, and has anxiety (mental health hashtags)
- Frequent Amazon reviews under the same email → Phone model identified

---

### 🥉 Phase 3: Attack Surface Hypothesis

- Phone OS: Android (older version, not patched)
- Cloud use: Google Drive + Dropbox (based on GitHub and LinkedIn)
- Weak points:
  - May use reused passwords (email in breach)
  - Uses Starbucks public WiFi
  - Smart devices at home (Instagram home photos show Alexa, smart bulbs)

---

## 💀 Endgame Scenarios (Hypothetical)

- **Social Engineering**: Pose as Amazon support — “Need OTP to verify unusual login.”
- **Location Mapping**: Physical presence traceable via geo-tagged habits
- **Credential Stuffing**: Use old password leak across Gmail, Dropbox, GitHub
- **Device Exploitation**: Public WiFi injection attack at Starbucks
- **Metadata Mining**: Extract EXIF from old images to pinpoint home GPS

---

## 🔐 Conclusion

OSINT isn't theory — it's **digital surveillance without the van**.  
Victim X was never “hacked.” He was simply **watched**.

> In a world oversharing every byte, silence becomes the last firewall.

---

## 🧠 Tools Used (All Legal)

- Google Dorks  
- Instagram Scraper  
- Wayback Machine  
- HaveIBeenPwned  
- GitHub commits search  
- EXIFTools  
- Maltego CE  
- Sherlock + Recon-ng

---

## 🧩 Countermeasures for Victim X

- Purge metadata from photos  
- Disable geo-tagging  
- Don’t reuse usernames  
- Use different handles for GitHub, socials  
- Use VPN on public WiFi  
- Opt-out from data brokers  
- Treat email like an SSN

---

