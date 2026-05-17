# Wazuh Installation on Ubuntu Server 22.04.5

## Step 1 — Update Ubuntu

```bash
sudo apt update && sudo apt upgrade -y
```

---

# Step 2 — Install curl

```bash
sudo apt install curl -y
```

---

# Step 3 — Download Wazuh Installer

```bash
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
```

---

# Step 4 — Install Wazuh

```bash
sudo bash wazuh-install.sh -a
```

This installs:
- Wazuh Manager
- Wazuh Indexer
- Wazuh Dashboard

---

# Step 5 — Verify Services

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```

All services should display:

```text
active (running)
```

---

# Step 6 — Open Dashboard

```text
https://SERVER-IP
```

Example:

```text
https://192.168.47.131
```

---

# Step 7 — Login

Username:
```text
admin
```

Password:
```text
Generated during installation
```
