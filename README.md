# 🛡️ Cybersecurity Internship – Phase 1 Report

**Intern:** Rulane Hlongwani  
**Focus:** Virtual Cybersecurity Lab Setup, Log Analysis, and Threat Detection  
**Date:** July 2025  

---

## 🔧 Lab Environment

I built a full cybersecurity lab using VirtualBox with the following virtual machines:

- **Kali Linux** (Main operations, SSH, documentation, scanning)
- **Ubuntu 1** – Hosting OpenCart web server
- **Ubuntu 2** – Reserved for future Linux attacks or services
- **Windows 10 x2** – One connected to Wazuh agent for log collection
- **Parrot OS** – Alternate attacking distro
- **Security Onion** – Passive monitoring and IDS setup
- **pfSense** – Firewall and network segmentation
- **Wazuh Server** – Centralized logging, SIEM dashboard
- **Metasploitable 2** – Vulnerable machine for exploitation practice

---

## 🛒 OpenCart Installation

On **Ubuntu 1**, I installed OpenCart for web-based threat simulations:

- Installed Apache, MySQL, PHP (LAMP stack)
- Installed OpenCart from official repo
- Confirmed it's accessible from Kali/Windows browsers

📸 _Screenshots saved in_ `screenshots/opencart/`

---

## 🔐 Wazuh Configuration

On **Wazuh Server VM:**

- Installed Wazuh server & dashboard
- Opened necessary ports
- Added SSH key access from Kali

On **Windows 10 VM (Agent):**

- Installed Wazuh Agent
- Connected agent to Wazuh Server (via manager IP)
- Configured `agent-auth` and verified status

📸 _Screenshots saved in_ `screenshots/wazuh/`

---

## 🔁 Connectivity Tests

- ✅ SSH from Kali to Wazuh server
- ✅ Access OpenCart from Parrot, Kali, and Windows
- ✅ View agent logs on Wazuh dashboard

---

## 📁 Files Included

- `README.md` – This document
- `/screenshots/` – Visual evidence of each setup step
- Any `.sh` or `.conf` files used for configuration

---

## ✅ Next Steps (Phase 2)

- Add Security Onion log integration
- Add pfSense logs to Wazuh
- Simulate real attacks using Metasploit
- Build detection rules for brute force, web attacks, etc.
- Automate incident alerting

---

_This marks the completion of Phase 1. I'm pushing this work to GitHub to track progress and share my learning journey._
