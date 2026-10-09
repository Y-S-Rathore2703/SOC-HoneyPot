 <div align="center">

# 🛡️ WAZUH HONEYPOT SOC LAB

### `Detect. Investigate. Defend.`

**A hands-on cybersecurity home lab for security monitoring, log analysis, and threat detection.**

![Status](https://img.shields.io/badge/STATUS-IN%20PROGRESS-00d68f?style=for-the-badge)
![Focus](https://img.shields.io/badge/FOCUS-DEFENSIVE%20SECURITY-00bfff?style=for-the-badge)
![Platform](https://img.shields.io/badge/PLATFORM-VIRTUALBOX-183A61?style=for-the-badge\&logo=virtualbox\&logoColor=white)

</div>

---

## `01 // ABOUT THE PROJECT`

This project is a personal cybersecurity lab built with **Oracle VirtualBox and Wazuh** to explore how security monitoring works in a controlled environment.

The goal is to build a honeypot-based lab, collect security events, monitor activity, and investigate alerts using defensive security tools.

I'm documenting the process from initial setup to event investigation to develop practical Linux, SIEM, and threat-detection skills.

## `02 // OBJECTIVES`

* 🖥️ Build an isolated virtual lab environment.
* 🛡️ Explore Wazuh SIEM and endpoint security monitoring.
* 🍯 Learn honeypot concepts and observe controlled interactions.
* 📊 Collect and analyze system and security logs.
* 🔎 Investigate alerts and understand suspicious activity.
* 📝 Document configurations, findings, and troubleshooting.

## `03 // LAB ARCHITECTURE`

```text
             VIRTUAL LAB ENVIRONMENT
          ┌──────────────────────────┐
          │     Oracle VirtualBox    │
          └────────────┬─────────────┘
                       │
             Isolated Lab Network
                       │
          ┌────────────┴─────────────┐
          │                          │
  ┌───────▼────────┐       ┌─────────▼────────┐
  │ Honeypot /     │       │ Wazuh Monitoring │
  │ Test Endpoint  │──────▶│ & SIEM           │
  └────────────────┘ Logs  └─────────┬────────┘
                                     │
                            ┌────────▼────────┐
                            │ Alerts &        │
                            │ Investigation   │
                            └─────────────────┘
```

*Planned architecture — the components and log flow will be updated as the lab is implemented.*

## `04 // TECH STACK`

<div align="center">

![Ubuntu](https://img.shields.io/badge/Ubuntu-Linux-E95420?style=for-the-badge\&logo=ubuntu\&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-4A90E2?style=for-the-badge)
![VirtualBox](https://img.shields.io/badge/Oracle-VirtualBox-183A61?style=for-the-badge\&logo=virtualbox\&logoColor=white)
![Networking](https://img.shields.io/badge/Virtual-Networking-00A98F?style=for-the-badge)
![Security](https://img.shields.io/badge/Focus-Threat%20Detection-111111?style=for-the-badge)

</div>

## `05 // PROJECT ROADMAP`

* [ ] **Phase 1:** Prepare the VirtualBox environment.
* [ ] **Phase 2:** Configure virtual machines and network isolation.
* [ ] **Phase 3:** Install and explore Wazuh.
* [ ] **Phase 4:** Connect an endpoint and verify log collection.
* [ ] **Phase 5:** Deploy a controlled honeypot.
* [ ] **Phase 6:** Generate safe test activity and analyze alerts.
* [ ] **Phase 7:** Document findings and lessons learned.

## `06 // WHAT I'M LEARNING`

| Area              | Practical learning                                |
| ----------------- | ------------------------------------------------- |
| Linux             | Commands, processes, services, and logs           |
| Networking        | Virtual networks, ports, and traffic flow         |
| SIEM              | Event collection, alerting, and dashboards        |
| Threat Detection  | Identifying and investigating suspicious activity |
| Incident Analysis | Reviewing evidence and documenting findings       |

## `07 // REPOSITORY STRUCTURE`

```text
wazuh-honeypot-soc-lab/
├── README.md
├── docs/
│   ├── day-1-checklist.md
│   ├── setup-guide.md
│   └── investigation-notes.md
├── screenshots/
│   └── README.md
├── configs/
│   └── README.md
└── .gitignore
```

*Configuration examples, screenshots, and notes will be added as the project progresses. Empty folders may need a placeholder README file to appear on GitHub.*

## `08 // SECURITY & ETHICS`

* All experiments are conducted in an authorized lab environment.
* Vulnerable services should remain isolated from public networks.
* No real credentials or sensitive data will be committed.
* Test activity will be controlled and used for defensive learning.

## `09 // PROJECT STATUS`

**Current stage:** Initial lab preparation.

The project is being developed step by step, with setup notes, screenshots, troubleshooting, and investigation results documented along the way.

---

<div align="center">

### `DETECT • INVESTIGATE • DEFEND`

*Learning cybersecurity by building, testing, and analyzing.*

**Created by Yuvraj Singh Rathore**

[GitHub](https://github.com/Y-S-Rathore2703) · [LinkedIn](https://www.linkedin.com/in/yuvraj-singh-rathore-327471334/) · [TryHackMe](https://tryhackme.com/p/Y.S.Rathore)

</div>
