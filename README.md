![Banner](profile_banner_maxime_belliard.svg)

<div align="center">

[![RNCP](https://img.shields.io/badge/RNCP%20Level%207-Cybersecurity%20Solutions%20Development-1A1A2E?style=flat-square)](https://www.francecompetences.fr/recherche/rncp/38463/)
[![PECB ISO 27001](https://img.shields.io/badge/PECB-ISO%2027001%20Provisional%20Implementer-C8102E?style=flat-square)](https://www.pecb.com)
[![PECB EBIOS](https://img.shields.io/badge/PECB-EBIOS%20Provisional%20Risk%20Manager-C8102E?style=flat-square)](https://www.pecb.com)
[![ISC2 CC](https://img.shields.io/badge/ISC2-Certified%20in%20Cybersecurity-00A651?style=flat-square&logo=isc2&logoColor=white)](https://www.isc2.org)

</div>

---

## 👋 About Me

I hold a French **RNCP Level 7** qualification in cybersecurity solutions development (EQF 7, Master's level) and I'm looking to join an **in-house security team** where I can both implement and analyse cybersecurity solutions — from technical hardening to governance.

Before moving into cybersecurity, I spent years as a **QSE (quality, safety, environment) manager and logistics operations leader**, which gave me a strong foundation in process discipline, regulatory compliance, and risk management — including **OT/IT environments**. I bring that operational mindset directly into security work.

What I can show today:
- 🏢 **Identity & Access Management** — Active Directory OU design, GPO hardening aligned with CIS Benchmarks, PingCastle assessment
- 🔍 **SIEM & Threat Detection** — Wazuh agents, custom decoder and rules, MITRE ATT&CK mapping, detections validated with controlled tests
- 🔥 **Network Security** — pfSense segmentation (WAN / LAN / DMZ, default-deny), Suricata IDS/IPS, OpenVAS vulnerability scanning
- 📋 **GRC** — ISO 27001 and EBIOS RM (PECB), NIS2 — technical controls justified against the frameworks

---

## 🎓 Certifications

| Certification | Issuer | Year |
|---|---|---|
| Expert en développement de solutions de cybersécurité — [RNCP 38463](https://www.francecompetences.fr/recherche/rncp/38463/), Level 7 (EQF 7) | AN21 / CSB School | 2024 |
| ISO/IEC 27001 Provisional Implementer | PECB | 2024 |
| EBIOS Provisional Risk Manager | PECB | 2024 |
| Certified in Cybersecurity (CC) | ISC2 | 2026 |

---

## 🏢 LogiSecure SA — The Lab Scenario

All labs simulate the security programme of **LogiSecure SA**, a fictional Belgian parcel logistics operator for B2B e-commerce (500 employees, Brussels HQ, automated sorting conveyors on the OT side). As a courier service provider it is an **NIS2** important entity, and it uses **ISO 27001** and **IEC 62443** as reference frameworks. Each project extends the same environment instead of starting from scratch.

**Built so far:** Active Directory `lab.local` · pfSense perimeter (WAN / LAN / DMZ) · Suricata IDS/IPS · Wazuh SIEM · OpenVAS

📌 Programme hub — company context and lab architecture: **[logisecure-enterprise-security-program](https://github.com/MaxBell10/logisecure-enterprise-security-program)**

---

## 🗂️ Projects

> A project is listed once its repository is published, plus the one in progress. Every figure below is evidenced in its repository.

| Repository | Status | Evidenced results |
|---|---|---|
| [logisecure-active-directory](https://github.com/MaxBell10/logisecure-active-directory) | ✅ Completed | AD domain with OU design · 4 GPOs (password, lockout, audit, hardening) · Wazuh agents on DC01 and WKS01 · custom MITRE-mapped rules · PingCastle risk reduced on Privileged Accounts (50 → 40) and Stale Objects (41 → 36) |
| [logisecure-pfsense-segmentation](https://github.com/MaxBell10/logisecure-pfsense-segmentation) | ✅ Completed | 12 firewall rules, default-deny on every interface · DMZ→LAN traffic blocked, shown in firewall logs · Suricata scan alerts decoded in Wazuh and mapped to T1046 · OpenVAS validated against nmap |
| logisecure-ebios-rm-assessment | 🔄 In progress | EBIOS RM risk assessment of LogiSecure SA |

### 🔎 Featured Write-up

**[The flagship detection rule never fired — found four months later](https://github.com/MaxBell10/logisecure-active-directory/blob/main/lessons_learned.md#the-flagship-detection-rule-never-fired--found-four-months-later)**

My custom T1110 rule shared its ID with an example rule that Wazuh ships by default, so Wazuh kept the example and dropped mine — for four months, with one unread warning line as the only signal. I found it during the pfSense project and proved the fix with the same controlled failed logon, before and after. The lesson: a detection is proven by making it fire, not by showing that the file exists.

---

## ⚖️ Frameworks Applied in the Labs

| Framework | Where it is applied |
|---|---|
| **MITRE ATT&CK** | Detections mapped to T1046 (Suricata scan alerts in Wazuh), T1078 and T1087 (custom Wazuh rules) · Mitigations for T1110 (account lockout) and T1557 (LLMNR disabled) |
| **CIS Benchmarks** | GPO hardening — password and lockout policies, NTLMv2 only, SMB signing |
| **ISO 27001:2022 · NIS2 Art. 21** | Default-deny firewall rules justified against ISO 27001 A.8.20 and NIS2 Art. 21 |

---

## 🛠️ Tools & Technologies

![Windows Server](https://img.shields.io/badge/Windows%20Server%202022-0078D6?style=flat-square&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active%20Directory-0078D6?style=flat-square&logo=microsoft&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh%20SIEM-4B5EAA?style=flat-square)
![pfSense](https://img.shields.io/badge/pfSense-212121?style=flat-square)
![Suricata](https://img.shields.io/badge/Suricata%20IDS%2FIPS-EF6C00?style=flat-square)
![OpenVAS](https://img.shields.io/badge/OpenVAS-4EAA25?style=flat-square)
![Nmap](https://img.shields.io/badge/Nmap-4682B4?style=flat-square)
![PingCastle](https://img.shields.io/badge/PingCastle-2B2D42?style=flat-square)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=flat-square&logo=virtualbox&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

---

<div align="center">

*All lab environments simulate the fictional enterprise LogiSecure SA, used solely for educational and portfolio purposes.*

</div>
