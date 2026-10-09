# 🛡️ DAY 01 — LAB RECONNAISSANCE

<div align="center">

![Phase](https://img.shields.io/badge/PHASE-01-00D68F?style=for-the-badge)
![Status](https://img.shields.io/badge/STATUS-IN_PROGRESS-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/FOCUS-ENVIRONMENT_SETUP-0078D4?style=for-the-badge)

**PROJECT:** Wazuh Honeypot SOC Lab
**OPERATOR:** Yuvraj Singh Rathore
**PLATFORM:** Oracle VirtualBox · Ubuntu Linux
**ESTIMATED TIME:** 45–60 minutes

</div>

---

## `01 // MISSION BRIEFING`

> Before building a security monitoring lab, understand the environment you're working in.

Today's mission is to inspect the existing Ubuntu virtual machine, identify its available resources, examine its current network configuration, and prepare the documentation needed for the upcoming Wazuh deployment.

### Mission objectives

* [ ] Inspect the existing virtual machine.
* [ ] Identify OS, CPU, RAM, and storage.
* [ ] Review current network settings.
* [ ] Plan a controlled lab environment.
* [ ] Document findings and save evidence to GitHub.

---

## `02 // PHASE ALPHA — REPOSITORY SETUP`

**Objective:** Establish a clean project documentation structure.

* [ ] Create the GitHub repository.
* [ ] Add the main `README.md`.
* [ ] Create the `docs/` directory.
* [ ] Add this checklist.
* [ ] Prepare a `screenshots/` directory.

**Expected output:** A structured repository ready to document the lab.

---

## `03 // PHASE BRAVO — VIRTUALBOX INSPECTION`

**Objective:** Understand the existing virtual machine before making changes.

### Tasks

* [ ] Open Oracle VirtualBox.
* [ ] Locate the existing Ubuntu VM.
* [ ] Record its status: Powered Off or Running.
* [ ] Open `Settings → System → Motherboard`.
* [ ] Record the allocated RAM.
* [ ] Open `Settings → System → Processor`.
* [ ] Record the allocated CPU cores.
* [ ] Open `Settings → Storage`.
* [ ] Inspect the virtual disk configuration.
* [ ] Capture a screenshot of the VM configuration.

### Environment inventory

| Component     | Observation        |
| ------------- | ------------------ |
| Host OS       | Windows            |
| Hypervisor    | Oracle VirtualBox  |
| Guest OS      | Pending inspection |
| VM status     | Pending inspection |
| Allocated RAM | Pending inspection |
| CPU cores     | Pending inspection |
| Virtual disk  | Pending inspection |

---

## `04 // PHASE CHARLIE — LINUX RECONNAISSANCE`

**Objective:** Collect basic system information from Ubuntu.

Open the Ubuntu terminal and run the following commands.

### 1. Identify the operating system

```bash
cat /etc/os-release
```

**Purpose:** Identify the Ubuntu version and OS details.

* [ ] Command executed
* [ ] Version recorded

### 2. Inspect memory usage

```bash
free -h
```

**Purpose:** View total, used, and available memory.

* [ ] Command executed
* [ ] Memory details recorded

### 3. Inspect filesystem capacity

```bash
df -h
```

**Purpose:** Check filesystem sizes and available disk space.

* [ ] Command executed
* [ ] Root filesystem space recorded

### 4. Inspect CPU information

```bash
lscpu
```

**Purpose:** Identify CPU architecture and processors visible to Ubuntu.

* [ ] Command executed
* [ ] CPU details recorded

### 5. Inspect network interfaces

```bash
ip addr
```

**Purpose:** Identify network interfaces and assigned IP addresses.

* [ ] Command executed
* [ ] Active interfaces identified
* [ ] Network details recorded privately

---

## `05 // PHASE DELTA — NETWORK ASSESSMENT`

**Objective:** Understand how the virtual machine connects to the network.

### Tasks

* [ ] Open `VirtualBox → VM Settings → Network`.
* [ ] Inspect the current attachment mode.
* [ ] Record whether it uses NAT, Bridged, Host-only, or Internal Network.
* [ ] Identify which network mode is currently active.
* [ ] Document questions about future lab isolation.
* [ ] Avoid changing settings until the network plan is clear.

**Security note:** A honeypot can expose vulnerable services. Keep experiments isolated from untrusted networks until the required security controls are understood and configured.

### Network assessment

| Property             | Result             |
| -------------------- | ------------------ |
| Current network mode | Pending inspection |
| Active interface     | Pending inspection |
| IP configuration     | Recorded privately |
| Isolation plan       | Pending design     |

---

## `06 // PHASE ECHO — EVIDENCE COLLECTION`

**Objective:** Build a verifiable record of the initial setup.

* [ ] Screenshot of the VirtualBox VM list.
* [ ] Screenshot of VM resource settings.
* [ ] Screenshot of Ubuntu running.
* [ ] Screenshot of terminal inspection commands.
* [ ] Save screenshots in `screenshots/`.
* [ ] Update this checklist with actual observations.
* [ ] Commit changes to GitHub.

**Evidence naming convention**

```text
screenshots/
├── day-01-virtualbox.png
├── day-01-ubuntu-terminal.png
└── day-01-system-resources.png
```

These are suggested filenames; use screenshots of your actual environment.

---

## `07 // FIELD NOTES`

### Observations

*Record what you discovered during the inspection.*

* Operating system:
* Available RAM:
* CPU allocation:
* Available disk space:
* Network mode:

### Challenges encountered

* No issues recorded yet.

### Questions for investigation

* How much memory will the monitoring components require?
* Should the honeypot and monitoring server run on separate VMs?
* How will logs reach Wazuh?
* Which network setup will provide suitable isolation?

---

## `08 // MISSION DEBRIEF`

### Definition of done

* [ ] Virtual machine identified.
* [ ] Operating system verified.
* [ ] CPU, RAM, and disk inspected.
* [ ] Network mode documented.
* [ ] Evidence captured and sanitized.
* [ ] Checklist committed to GitHub.

### Skills practiced

`Linux` · `Virtualization` · `System Inspection` · `Networking` · `Technical Documentation`

### Mission status

**IN PROGRESS** — Mark complete only after verifying the tasks and recording the findings.

---

## `09 // NEXT MISSION`

### DAY 02 — RESOURCE PLANNING & NETWORK DESIGN

Next, we'll review available host resources, decide how many virtual machines are practical, and design the lab network before installing Wazuh or deploying a honeypot.

<div align="center">

**`RECONNAISSANCE → PLANNING → DEPLOYMENT`**

*Wazuh Honeypot SOC Lab*
*Learn · Practice · Analyze · Defend*

</div>

