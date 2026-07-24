# 🛡️ Project 01 – File Integrity Monitoring (FIM) using Wazuh SIEM

> Detecting file creation, modification, and deletion on a Windows endpoint using Wazuh File Integrity Monitoring (FIM).

---

## 📌 Project Overview

This project demonstrates how **Wazuh SIEM** monitors file system changes on a Windows endpoint. File Integrity Monitoring (FIM) helps security teams detect unauthorized changes to critical files, supporting threat detection and incident investigation.

---

## 🎯 Objectives

- Configure File Integrity Monitoring (FIM) in Wazuh.
- Monitor file creation, modification, and deletion.
- Generate real-time alerts.
- Investigate alerts using the Wazuh Dashboard.
- Document findings through an incident report.

---

## 🖥️ Lab Environment

| Component | Technology |
|-----------|------------|
| SIEM | Wazuh 4.x |
| Manager | Ubuntu Server |
| Endpoint | Windows 10 |
| Virtualization | VirtualBox |

---

## 🏗️ Lab Architecture

```text
                 +----------------------+
                 |    Ubuntu Server     |
                 |    Wazuh Manager     |
                 +----------+-----------+
                            |
                     Wazuh Agent
                            |
                 +----------+-----------+
                 |     Windows 10       |
                 |  File Monitoring     |
                 +----------------------+
```

---

## ⚙️ Configuration

- Installed Wazuh Manager.
- Connected Windows Agent.
- Enabled File Integrity Monitoring.
- Configured monitored directories.
- Verified agent communication.

---

## 🧪 Test Scenario

1. Create a test file.
2. Modify the file.
3. Delete the file.
4. Observe alerts in the Wazuh Dashboard.

---

## 🚨 Detection Results

✅ File Created

✅ File Modified

✅ File Deleted

All events were successfully detected and logged by Wazuh.

---

## 📸 Screenshots

> Store all screenshots inside the **Screenshots/** folder.

| Screenshot | Description |
|------------|-------------|
| Lab-Setup.png | Home Lab Topology |
| Agent-Connected.png | Windows Agent Connected |
| File-Created.png | File Creation Alert |
| File-Modified.png | File Modification Alert |
| File-Deleted.png | File Deletion Alert |
| Alert-Details.png | Wazuh Alert Details |

---

## 📄 Incident Report

The complete incident report is available here:

📄 **[Incident Report](Incident-Report.md)**

---

## 🧠 Skills Demonstrated

- Wazuh SIEM
- File Integrity Monitoring (FIM)
- Windows Security
- Log Analysis
- Incident Investigation
- Threat Hunting

---

## 📚 MITRE ATT&CK

Although this project focuses on monitoring file changes, FIM can assist analysts during investigations involving persistence, defense evasion, and impact techniques.

---

## ✅ Project Outcome

Successfully configured Wazuh File Integrity Monitoring to detect and investigate file system changes on a Windows endpoint, strengthening practical SOC Analyst skills in security monitoring and incident analysis.

---

### 👨‍💻 Author

**Muhammad Tashfeen**

Cyber Security Student | Aspiring SOC Analyst

GitHub: https://github.com/YOUR_USERNAME

LinkedIn: https://linkedin.com/in/YOUR_PROFILE
