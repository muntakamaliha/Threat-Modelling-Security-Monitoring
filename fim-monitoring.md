# File Integrity Monitoring (FIM)

## Overview

File Integrity Monitoring (FIM) is a security feature that continuously monitors files and directories for unauthorized changes. Wazuh detects file creation, modification, deletion, permission changes, and hash changes, helping security teams identify suspicious activities and maintain system integrity.

---

# Objectives

- Monitor critical files
- Detect unauthorized changes
- Generate security alerts
- Maintain file integrity
- Support incident investigation

---

# Accessing File Integrity Monitoring

1. Open the Wazuh Dashboard.
2. Log in using an administrator account.
3. Navigate to **Modules → Integrity Monitoring**.
4. Review the generated file events.

---

# Demonstration 1: File Creation

## Steps

1. Create a new file named `demo.txt`.
2. Save the file.

## Expected Result

- File Created
- Timestamp Recorded
- Agent Name Displayed


# Demonstration 2: File Modification

## Steps

1. Open `demo.txt`.
2. Add new content.
3. Save the file.

## Expected Result

- File Modified
- SHA Hash Updated
- Timestamp Updated



# Demonstration 3: File Deletion

## Steps

1. Delete `demo.txt`.

## Expected Result

- File Deleted
- Security Event Generated



# Information Collected by Wazuh

For each monitored event, Wazuh records:

- File Path
- Event Type
- Timestamp
- Agent Name
- User (when available)
- SHA1 / SHA256 Hash
- File Size

---

# Benefits of File Integrity Monitoring

- Detects unauthorized file changes
- Protects critical system files
- Supports compliance requirements
- Helps investigate security incidents
- Improves endpoint visibility

---

# Conclusion

The File Integrity Monitoring module successfully detected file creation, modification, and deletion events during this project. These demonstrations confirmed that Wazuh can continuously monitor important files and generate alerts whenever changes occur.
