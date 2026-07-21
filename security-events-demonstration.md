# Security Events Demonstration

## Overview

This document demonstrates the security events generated during the Wazuh SIEM project. Each event was intentionally created to verify that Wazuh successfully collected, analyzed, and displayed the logs in the Wazuh Dashboard.

---

# Event 1: Failed Login Attempt

## Objective

Generate a Windows authentication failure.

## Steps

1. Lock or sign out of the Windows system.
2. Enter an incorrect password five times.
3. Log in using the correct password.

## Expected Result

- Event ID: 4625
- Authentication Failure
- Security Event Generated

## Dashboard Location

Security Events → Threat Hunting → Discover


# Event 2: Successful Login

## Steps

1. Log in with the correct password.

## Expected Result

- Event ID: 4624
- Successful Authentication

## Dashboard Location

Security Events


# Event 3: File Creation

## Steps

1. Create a file named `demo.txt`.

## Expected Result

- File Created
- FIM Event Generated

## Dashboard Location

Integrity Monitoring


# Event 4: File Modification

## Steps

1. Open `demo.txt`.
2. Add new text.
3. Save the file.

## Expected Result

- File Modified
- Hash Changed

## Dashboard Location

Integrity Monitoring


# Event 5: File Deletion

## Steps

1. Delete `demo.txt`.

## Expected Result

- File Deleted

## Dashboard Location

Integrity Monitoring


# Event 6: PowerShell Execution

## Steps

1. Open Windows PowerShell.

## Expected Result

- Process Creation Event
- 

# Event 7: Command Prompt Execution

## Steps

1. Open Command Prompt.

## Expected Result

- Process Creation Event


# Event 8: User Account Creation

## Command

```cmd
net user demo Password123! /add
```

## Expected Result

- User Account Created

---

# Event 9: User Account Deletion

## Command

```cmd
net user demo /delete
```

## Expected Result

- User Account Deleted

---

# Event 10: Windows Service Stop and Start

## Commands

```cmd
net stop spooler
net start spooler
```

## Expected Result

- Service Stopped
- Service Started

---

# Conclusion

The generated security events confirmed that Wazuh successfully monitored authentication activities, file integrity changes, process execution, user management, and Windows service events. These demonstrations validate the effectiveness of Wazuh as a SIEM solution for centralized log collection and security monitoring.
