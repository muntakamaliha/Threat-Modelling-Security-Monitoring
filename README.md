# Threat Modeling and Security Monitoring using Wazuh SIEM

## Project Overview

This project demonstrates the deployment of a Security Information and Event Management (SIEM) solution using Wazuh. The environment consists of an Ubuntu Server hosting the Wazuh Manager, Wazuh Indexer, and Wazuh Dashboard, with Windows 11 and Kali Linux configured as monitored endpoints.

The project focuses on centralized log management, threat detection, file integrity monitoring, authentication monitoring, and security event analysis in a virtual lab environment.

---

# Author

**Name:** Muntaka Maliha Rahman

---

# Project Objectives

- Deploy Wazuh SIEM on Ubuntu Server
- Configure Windows 11 and Kali Linux as Wazuh Agents
- Monitor security events from multiple endpoints
- Demonstrate File Integrity Monitoring (FIM)
- Perform Threat Hunting using Wazuh Dashboard
- Analyze authentication and system events
- Explore Wazuh security modules
- Document the complete deployment process

---

# Technologies Used

- Ubuntu Server 24.04 LTS
- Wazuh SIEM
- Wazuh Dashboard
- Wazuh Manager
- Wazuh Indexer
- Windows 11
- Kali Linux
- Oracle VirtualBox
- OpenSSH
- MobaXterm / PuTTY
- Git
- GitHub

---

# Lab Environment

| Component | Details |
|------------|------------|
| Hypervisor | Oracle VirtualBox |
| SIEM Platform | Wazuh |
| Server | Ubuntu Server 24.04 LTS |
| Endpoint 1 | Windows 11 |
| Endpoint 2 | Kali Linux |
| Network Mode | Bridged Adapter |

---

# Project Workflow

1. Install Ubuntu Server
2. Configure Network
3. Enable SSH
4. Connect remotely using MobaXterm / PuTTY
5. Install Wazuh
6. Verify Wazuh Services
7. Configure Windows Agent
8. Configure Kali Linux Agent
9. Generate Security Events
10. Perform Threat Hunting
11. Demonstrate File Integrity Monitoring
12. Upload Project to GitHub

---

# Repository Contents

| File | Description |
|------|-------------|
| README.md | Project overview |
| ubuntu-server-installation.md | Ubuntu installation guide |
| wazuh-installation.md | Wazuh installation guide |
| commands-used.md | Commands used during installation |
| security-events-demonstration.md | Security event generation |
| dashboard-features.md | Dashboard feature explanation |
| threat-hunting.md | Threat hunting examples |
| fim-monitoring.md | File Integrity Monitoring |
| conclusion.md | Project conclusion |

---

# Wazuh Dashboard Modules Demonstrated

- Security Events
- Threat Hunting
- Discover
- File Integrity Monitoring (FIM)
- MITRE ATT&CK
- Inventory
- Vulnerability Detection
- Agent Management

---

# Security Events Demonstrated

- Failed Login (Event ID 4625)
- Successful Login (Event ID 4624)
- File Creation
- File Modification
- File Deletion
- PowerShell Execution
- Command Prompt Execution
- User Account Creation
- User Account Deletion
- Windows Service Start
- Windows Service Stop

---

# Wazuh Services Verification

```bash
sudo systemctl status wazuh-manager

sudo systemctl status wazuh-indexer

sudo systemctl status wazuh-dashboard
```

All services were successfully running.

---

# Threat Hunting Examples

```text
event.code:4625

event.code:4624

agent.name:"Windows"

rule.level>=7

rule.groups:syscheck

syscheck.path:*demo.txt
```

---

# File Integrity Monitoring

The following actions were successfully monitored:

- File Created
- File Modified
- File Deleted
- Hash Changes
- Timestamp Changes

---

# Screenshots

This repository includes screenshots demonstrating:

- Ubuntu Server Installation
- Wazuh Installation
- Dashboard Login
- Active Agents
- Security Events
- Threat Hunting
- Discover
- File Integrity Monitoring
- MITRE ATT&CK
- Inventory
- Vulnerability Detection

---

# System Requirements

| Component | Requirement |
|------------|------------|
| CPU | 2 Cores or higher |
| RAM | 4 GB Minimum |
| Storage | 50 GB |
| Operating System | Ubuntu Server |

---

# Conclusion

This project successfully demonstrates the deployment of a Wazuh SIEM environment for centralized security monitoring. Windows 11 and Kali Linux endpoints were integrated with the Wazuh Manager, enabling real-time log collection, authentication monitoring, file integrity monitoring, and threat hunting. The project showcases how SIEM technology can be used to detect, investigate, and monitor security events in a virtual SOC environment.
