# Wazuh Dashboard Features

## Overview

The Wazuh Dashboard provides a centralized platform for monitoring, analyzing, and investigating security events collected from connected endpoints. It helps security analysts identify suspicious activities, perform threat hunting, and monitor system integrity in real time.

---

# 1. Dashboard Home

The Dashboard Home provides an overview of the Wazuh deployment, including connected agents, event statistics, alerts, and monitoring summaries.

**Purpose**

- View overall system health
- Monitor alert activity
- Access all Wazuh modules


# 2. Agents

The Agents module displays all registered endpoints connected to the Wazuh Manager.

Information displayed includes:

- Agent Name
- Operating System
- Agent Version
- Status (Active / Disconnected)
- Last Keep Alive


# 3. Security Events

The Security Events module collects and displays logs from monitored endpoints.

Examples:

- Failed Login
- Successful Login
- Windows Security Events
- Linux Authentication Logs
- Service Events


# 4. Threat Hunting

Threat Hunting allows analysts to search collected logs using filters and queries.

Example Queries

```
event.code:4625
```

```
event.code:4624
```

```
agent.name:"Windows"
```

```
rule.level>=7
```

```
rule.groups:syscheck
```


# 5. Discover

Discover displays raw events received by Wazuh.

Useful filters include:

- Agent Name
- Event Code
- Rule Level
- File Path
- Timestamp


# 6. File Integrity Monitoring (FIM)

File Integrity Monitoring detects changes made to monitored files.

Supported events:

- File Created
- File Modified
- File Deleted
- Permission Changed
- Hash Changed


# 7. MITRE ATT&CK

This module maps detected events to the MITRE ATT&CK framework.

Examples include:

- Initial Access
- Execution
- Persistence
- Credential Access
- Privilege Escalation


# 8. Inventory

The Inventory module provides information about monitored systems.

Information includes:

- Installed Software
- Operating System
- Hardware Information
- Running Processes


# 9. Vulnerability Detection

This module identifies known software vulnerabilities using CVE information.

Displayed information includes:

- CVE ID
- Severity
- Affected Package
- Risk Level


# Conclusion

The Wazuh Dashboard provides a complete Security Operations Center (SOC) interface for centralized monitoring, threat detection, security event analysis, file integrity monitoring, and vulnerability management.
