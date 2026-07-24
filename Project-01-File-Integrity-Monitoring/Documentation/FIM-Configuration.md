# File Integrity Monitoring (FIM) Documentation

## Purpose

The purpose of this project is to demonstrate how Wazuh File Integrity Monitoring (FIM) detects file system changes on a Windows endpoint. FIM helps SOC analysts identify unauthorized file creation, modification, and deletion.

---

# Technologies Used

- Wazuh SIEM
- Ubuntu Server
- Windows 10
- VirtualBox

---

# Lab Architecture

```
Windows 10 Agent
        │
        │ Wazuh Agent
        ▼
Ubuntu Server (Wazuh Manager)
        │
        ▼
Wazuh Dashboard
```

---

# Configuration

## Step 1: Install Wazuh Manager

Install and configure the Wazuh Manager on Ubuntu Server.

## Step 2: Connect Windows Agent

Register the Windows 10 endpoint with the Wazuh Manager and verify that the agent is active.

## Step 3: Enable File Integrity Monitoring

Configure Wazuh to monitor the required directories for file changes.

## Step 4: Restart Wazuh

Restart the Wazuh Manager to apply the configuration.

---

# Test Procedure

1. Create a new file.
2. Modify the file.
3. Delete the file.
4. Open the Wazuh Dashboard.
5. Verify that alerts are generated for each action.

---

# Detection Results

The following events were successfully detected:

- File Created
- File Modified
- File Deleted

Each alert included:
- File path
- Event timestamp
- Agent name
- Rule information

---

# Investigation

The generated alerts were reviewed in the Wazuh Dashboard to verify:

- Event type
- Monitored file path
- Detection timestamp
- Alert severity
- Agent information

---

# Security Benefits

- Detects unauthorized file changes
- Supports threat hunting
- Improves visibility into endpoint activity
- Assists incident response investigations

---

# Skills Demonstrated

- Wazuh SIEM
- File Integrity Monitoring (FIM)
- Windows Security
- Log Analysis
- Threat Hunting
- Incident Investigation

---

# Outcome

The project successfully demonstrated Wazuh's ability to monitor critical file system changes in real time. File creation, modification, and deletion events were detected and analyzed, providing practical experience in security monitoring and incident investigation.
