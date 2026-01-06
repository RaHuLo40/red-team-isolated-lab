# Vulnerable Target: Metasploitable2

This document describes the intentionally vulnerable system used as the attack target in the red team home lab.

---

## 🧨 What Is Metasploitable2?

Metasploitable2 is a deliberately vulnerable Linux virtual machine designed for **penetration testing practice**.

It contains:
- Outdated services
- Weak configurations
- Known exploitable vulnerabilities

This makes it ideal for learning **offensive security techniques** in a controlled environment.

---

## ⚠️ Why Metasploitable2 Is Dangerous

Metasploitable2 should **never** be exposed to:
- The internet
- A corporate network
- A home LAN

Risks include:
- Remote code execution
- Unauthorized access
- Network compromise

For this reason, the machine is placed in a **fully isolated network**.

---

## 🌐 Network Configuration

- Network Mode: Host-Only / Internal Network
- Interface: `eth0`
- IP Address: Assigned via DHCP
- Internet Access: Disabled

This ensures the vulnerable services are accessible **only** to attacker machines inside the lab.

---

## 🔍 Verification

```bash
ifconfig
---

## 🧠 Security & Ethical Considerations

This system is used strictly for:
- Learning purposes
- Red team skill development
- Safe exploit experimentation

⚠️ Exploiting real systems without authorization is illegal and unethical.

---

## ✅ Summary

- Intentionally vulnerable target
- Fully isolated from external networks
- Used only for controlled red team exercises
