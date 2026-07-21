# Commands Used During the Project

This document contains the Linux, Wazuh, Windows, and Git commands used during the deployment and testing of the Wazuh SIEM environment.

---

# Ubuntu Update

```bash
sudo apt update
sudo apt upgrade -y
```

---

# Install Required Package

```bash
sudo apt install curl -y
```

---

# Download Wazuh Installer

```bash
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
```

---

# Install Wazuh

```bash
sudo bash wazuh-install.sh -a
```

---

# Verify Wazuh Services

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

---

# Restart Wazuh Services

```bash
sudo systemctl restart wazuh-manager
sudo systemctl restart wazuh-indexer
sudo systemctl restart wazuh-dashboard
```

---

# Check IP Address

```bash
ip a
```

or

```bash
hostname -I
```

---

# Verify SSH Service

```bash
sudo systemctl status ssh
```

---

# Windows Agent Verification

```powershell
Get-Service Wazuh
```

---

# Git Commands

```bash
git init
git add .
git commit -m "Complete Wazuh SIEM Project"
git branch -M main
git remote add origin https://github.com/<your-username>/Threat-Modelling-Security-Monitoring.git
git push -u origin main
```

---

# Notes

These commands were used during the installation, configuration, verification, and documentation of the Wazuh SIEM lab environment.
