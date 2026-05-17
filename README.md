# Wazuh Installation on Ubuntu Server 22.04.5
Manual setup of Wazuh on Ubuntu – full connection process. Created as a personal practice after following the lab manual and Linux command lessons from sir. Includes step-by-step commands and configuration.

## Author

- Name: Muntaka Maliha Rahman

---

# Project Objective

This project demonstrates the complete installation process of Ubuntu Server 22.04.5 and Wazuh SIEM. The server is remotely accessed using PuTTY and the project is uploaded to GitHub.

---

# Technologies Used

- Ubuntu Server 22.04.5 LTS
- Wazuh SIEM
- PuTTY
- GitHub
- VirtualBox / VMware

---

# Project Workflow

1. Install Ubuntu Server
2. Configure Network
3. Enable OpenSSH
4. Connect using PuTTY
5. Install Wazuh SIEM
6. Verify Services
7. Upload Project to GitHub

---

# Files Included

| File | Description |
|---|---|
| ubuntu-server-installation.md | Ubuntu Server installation steps |
| wazuh-installation.md | Wazuh installation process |
| commands-used.md | All commands used |
| conclusion.md | Final project conclusion |

---

# System Requirements

| Component | Requirement |
|---|---|
| CPU | 2 Core |
| RAM | 4 GB Minimum |
| Storage | 50 GB |
| OS | Ubuntu Server 22.04.5 |

---

# PuTTY Connection

Host:
```text
192.168.47.131
```

Port:
```text
22
```

---

# Wazuh Dashboard

```text
https://SERVER-IP
```

Example:
```text
https://192.168.47.131
```

---

# Verification

The following services were verified successfully:

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

All services were running successfully.

---

# Git Commands

```bash
git init
git add .
git commit -m "Complete Wazuh SIEM project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/wazuh-installation-ubuntu-server.git
git push -u origin main
```

---

# Conclusion

Wazuh SIEM was successfully installed on Ubuntu Server 22.04.5 and managed remotely using PuTTY.
