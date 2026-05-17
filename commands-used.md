# Commands Used in This Project

## Ubuntu Update

```bash
sudo apt update && sudo apt upgrade -y
```

---

## Install curl

```bash
sudo apt install curl -y
```

---

## Download Wazuh Installer

```bash
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
```

---

## Install Wazuh

```bash
sudo bash wazuh-install.sh -a
```

---

## Check Services

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

---

## Check IP Address

```bash
ip a
```

---

## Git Commands

```bash
git init
git add .
git commit -m "Complete Wazuh SIEM project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/wazuh-installation-ubuntu-server.git
git push -u origin main
```
