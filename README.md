HEAD
# 🛡️ Cybersecurity Projects – Phase 1 Report

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

# 🛍️ OpenCart Lab Setup – SIEM Internship Phase 1

Welcome to my lab project! This repository documents my hands-on journey setting up and installing **OpenCart** within a custom-built virtual lab as part of my **SIEM Internship – Phase 1**. This project involved real troubleshooting, Linux usage, file sharing via VirtualBox, and publishing everything using Git and GitHub.

---

## 🚀 Project Goals

* ✅ Set up a fully functioning OpenCart store on Ubuntu Linux
* ✅ Overcome VM errors (like low storage)
* ✅ Move to Kali Linux for better Git integration
* ✅ Learn and document every step in a clear and structured way
* ✅ Share the experience publicly as part of my growth

---

## 🧪 Lab Environment

* **Host OS:** Windows 10
* **VirtualBox VMs:** Ubuntu Linux & Kali Linux
* **Tools Used:** Apache, MySQL, PHP, Git, Nano, GitHub

---

## 🛠️ Key Steps Completed

### Ubuntu VM:

* Installed LAMP stack
* Created MySQL DB for OpenCart
* Downloaded & extracted `opencart-4.0.2.3`
* Launched and configured the store via browser

### Storage Issues:

* Faced full-disk problems
* Took screenshots
* Cleared up space and reinstalled VM

### Kali Linux:

* Installed Guest Additions
* Configured Shared Folder access
* Transferred screenshots from host to Kali
* Used Git CLI to upload everything to GitHub

---

## 📸 Screenshots

All setup steps are documented with screenshots — check the `OpenCart-Setup.md` file in this repo to see them all.

---

## 📄 Full Documentation

👉 [Click here to view OpenCart-Setup.md](./OpenCart-Setup.md)

---

## 🧠 Lessons Learned

* Real-world VM troubleshooting and recovery
* Installing and configuring eCommerce platforms
* Using Git and GitHub like a professional
* Power of documenting errors + fixes
* Confidence with Linux CLI tools

---

## 🙋‍♂️ Author

**Rulane Hlongwani**
Cybersecurity Intern | Linux Learner | GitHub Explorer
📫 Connect with me: [LinkedIn](https://www.linkedin.com/in/rlinemavuyangwa)

---

## ⭐️ If this inspired you, feel free to fork or follow!
 055a7f14c3bbccfa3f340a41fa6b25334cf7b8f1
