# Lab Usage Flow & Exploitation Roadmap

This document describes how the red team home lab is intended to be used and outlines a structured learning roadmap for offensive security practice.

---

## 🧭 Lab Usage Flow

The lab follows a realistic red team attack workflow:

1. Attacker machines (Kali / Parrot) are started
2. Network connectivity to the target is verified
3. Reconnaissance is performed
4. Vulnerabilities are identified
5. Exploitation is attempted
6. Post-exploitation techniques are practiced
7. The lab is reset for the next exercise

This structured flow mirrors real-world penetration testing methodology.

---

## 🔎 Phase 1: Reconnaissance

Goal: Identify live hosts, open ports, and running services.

Examples:
- Network discovery
- Port scanning
- Service version detection

(No exploits are launched at this stage.)

---

## 🧪 Phase 2: Vulnerability Identification

Goal: Map discovered services to known vulnerabilities.

Examples:
- Identifying outdated software
- Mapping services to CVEs
- Understanding misconfigurations

This phase focuses on **analysis, not exploitation**.

---

## 💥 Phase 3: Exploitation (Controlled)

Goal: Gain limited access to the vulnerable system in a safe environment.

Examples:
- Exploiting known vulnerable services
- Gaining a low-privilege shell

All exploitation remains:
- Fully isolated
- Fully authorized
- Educational only

---

## 🔓 Phase 4: Post-Exploitation

Goal: Understand the impact of a successful compromise.

Examples:
- Privilege escalation concepts
- Credential harvesting simulations
- Persistence awareness

This phase builds attacker mindset and defensive awareness.

---

## ♻️ Phase 5: Reset & Repeat

After each exercise:
- Virtual machines are reset or reverted
- Lessons learned are documented
- The next attack path is planned

This encourages iterative learning.

---

## 📈 Future Expansion Roadmap

Planned improvements to the lab:
- Add additional vul
