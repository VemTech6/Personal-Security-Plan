# 🔐 Personal Security Plan (PSP) – Dakhari Shorter


## 📝 Overview

This **Personal Security Plan (PSP)** outlines my approach to operational security as a cybersecurity student and aspiring Blue Team professional. It documents the tools, practices, and defensive strategies I personally use to protect my digital footprint — from system hardening and MFA to secure development, logging, and threat modeling.

Unlike theoretical coursework, this PSP reflects my real-world mindset: I don’t just study cybersecurity — I live it. Maintaining this plan helps me apply Blue Team principles to my own environment, improve my personal risk posture, and continuously adapt to evolving threats.

I created this PSP to demonstrate my commitment to good security hygiene, showcase my defensive thinking, and serve as a baseline for future personal and professional security improvements.


---

## 📱 Personal Device Security

- All personal devices (phone, laptop, VM host) are protected by:
  - Strong alphanumeric passwords + biometrics
  - Full disk encryption (BitLocker on Windows, FileVault on macOS)
  - Auto-lock timers enabled (2–5 mins idle)
- Mobile device runs:
  - App permission management
  - Encrypted messaging (Signal for sensitive comms)

---

## 🌐 Network Hygiene

- Home Wi-Fi secured with WPA2/WPA3 and MAC filtering  
- Guest network is isolated from internal LAN  
- DNS filtering via NextDNS and Pi-hole (when applicable)  
- Regular scans using:
  - `nmap` for open ports
  - Zeek for network traffic monitoring  
- VPN used on public Wi-Fi (Mullvad/ProtonVPN preferred)

---

## 💾 Data Management & Backups

- Critical files backed up to encrypted external drive + cloud (Proton Drive)
- All USB drives are scanned in isolated VM before use  
- GitHub projects scrubbed for sensitive metadata before uploading  
- Use of `.gitignore` and secrets management for all code repos

---

## 🛡️ Identity & Access Management

- MFA enabled on all accounts (prefer TOTP via Authy over SMS)  
- Password manager (Bitwarden) used with 20+ char generated passwords  
- SSH keys rotated every 6 months  
- Personal threat model reviewed quarterly

---

## 💬 Digital Footprint & OSINT Defense

- Regular checks of PII exposure on haveibeenpwned, Dehashed, and public breach sites  
- No personal email/phone used on public GitHub commits or submissions  
- Active monitoring of social media settings and exposure  
- Alias accounts used for public testing or community platforms when needed

---

## ⚙️ Personal Security Stack

- **SIEM:** Splunk, Wazuh  
- **Traffic Analysis:** Wireshark, Zeek  
- **Threat Intel:** VirusTotal, AbuseIPDB, Shodan  
- **Automation/Scripting:** Python, PowerShell  
- **Endpoint Security:** Windows Defender + Group Policy hardening

---

## 📈 Risk Assessment (Self)

| Category                  | Risk Level | Mitigation Strategy                      |
|---------------------------|------------|-------------------------------------------|
| Public GitHub exposure    | Medium     | Regularly review for API keys and PII     |
| Mobile app tracking       | Medium     | Limit app permissions; use tracker blockers |
| Social engineering        | High       | Ongoing awareness training + limited info sharing |
| Phishing/email compromise | High       | Email filters, URL inspection, link hover habits |
| USB/Removable drives      | Medium     | Only used in test VMs or with AV scanning  |



---

## 🚀 Ongoing Actions

- Continue rotating passwords every 90 days  
- Quarterly audit of GitHub and LinkedIn for exposed info  
- Maintain isolated VMs for malware/scripting tests  
- Expand on PSP based on threat model changes and role evolution  

---

> _“People always make the best exploits.”_  
> — Elliot Alderson, *Mr. Robot*


