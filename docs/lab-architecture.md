# Lab Architecture & Network Isolation

This document explains the **architecture** of the red team home lab and how network isolation is implemented to ensure safety.

---

## 🧱 Virtualization Platform

The lab is hosted on **VirtualBox**, which allows multiple operating systems to run simultaneously while remaining logically separated from the host system.

Virtual machines used:
- Kali Linux (Attacker)
- Parrot OS (Attacker)
- Metasploitable2 (Vulnerable Target)

---

## 🌐 Network Design

The lab uses an **isolated virtual network** to prevent:
- Accidental exposure of vulnerable services
- Attacks leaking into real networks
- Internet access from the vulnerable machine

### Network Mode Used
- **Host-Only Network** (or Internal Network)

This ensures:
- VMs can communicate **only with each other**
- No direct access to the internet
- No access to the host LAN

---

## 🔒 Isolation Strategy

| Machine | Network Access | Reason |
|------|---------------|-------|
| Kali Linux | Lab network only | Launch attacks safely |
| Parrot OS | Lab network only | Secondary attacker machine |
| Metasploitable2 | Lab network only | Prevent real-world exposure |

---

## 🧠 Why Isolation Matters in Red Team Labs

Metasploitable2 contains **deliberate vulnerabilities** such as:
- Weak credentials
- Outdated services
- Known exploitable CVEs

Running such systems without isolation could:
- Expose your real network
- Create legal and security risks

Isolation ensures:
- Safe learning
- Ethical experimentation
- Zero external impact

---

## ✅ Architecture Summary

- Fully offline attack lab
- No internet access for target
- Controlled attacker environment
- Safe for long-term red team practice
