# Ubuntu Server 22.04.5 Installation Process

## Step 1 — Download Ubuntu Server ISO

Official Website:

https://ubuntu.com/download/server

---

# Step 2 — Create Virtual Machine

Using:
- VirtualBox
- VMware

Recommended Configuration:

| Component | Value |
|---|---|
| RAM | 4 GB |
| CPU | 2 Core |
| Storage | 50 GB |

---

# Step 3 — Start Installation

Select:

```text
Install Ubuntu Server
```

---

# Step 4 — Choose Language

Example:
```text
English
```

---

# Step 5 — Configure Keyboard

Use default keyboard settings.

---

# Step 6 — Configure Network

Ubuntu automatically detects DHCP.

Check IP:
```bash
ip a
```

Example IP:
```text
192.168.47.131
```

---

# Step 7 — Configure Proxy

Leave empty.

---

# Step 8 — Configure Storage

Select:

```text
Use an entire disk
```

---

# Step 9 — Create User

Example:

| Field | Value |
|---|---|
| Name | Maliha |
| Server Name | wazuh-server |
| Username | maliha |

---

# Step 10 — Install OpenSSH Server

Select:

```text
Install OpenSSH Server
```

This enables remote SSH connection.

---

# Step 11 — Finish Installation

Select:
```text
Reboot Now
```

---

# Step 12 — Login

Login using username and password.

---

# Step 13 — Check IP Address

```bash
ip a
```

---

# Step 14 — Connect Using PuTTY

Host:
```text
192.168.47.131
```

Port:
```text
22
```
