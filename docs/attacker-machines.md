# Attacker Machines Setup (Kali Linux & Parrot OS)

This document describes the configuration and verification of the attacker machines used in the red team home lab.

---

## 🐉 Kali Linux (Primary Attacker)

Kali Linux is used as the **primary attacker machine** due to its extensive collection of offensive security tools.

### Network Configuration
- Network Mode: Host-Only / Internal Network
- Interface: `eth0`
- IP Address: Assigned via DHCP


## 🦜 Parrot OS (Secondary Attacker)

Parrot OS is used as a **secondary attacker machine** for alternative workflows and tool comparison.

### Network Configuration
- Network Mode: Host-Only / Internal Network
- Interface: `enp0s3`
- IP Address: Assigned via DHCP



### Verification
```bash
ip a 


