# ⚡ Project 04 – PowerShell Execution Detection using Wazuh SIEM

> Detecting PowerShell execution events using Wazuh SIEM for threat monitoring and incident investigation.

---

# 📌 Project Overview

This project demonstrates how Wazuh SIEM detects PowerShell execution events on a Windows endpoint. PowerShell is widely used by administrators but is also commonly abused by attackers for post-exploitation and malicious activities. Monitoring PowerShell execution helps SOC analysts identify suspicious behavior.

---

# 🎯 Objectives

- Monitor PowerShell execution events.
- Collect PowerShell logs using Wazuh.
- Investigate alerts in the Wazuh Dashboard.
- Map detections to the MITRE ATT&CK framework.
- Document the incident response process.

---

# 🖥️ Lab Environment

| Component | Technology |
|-----------|------------|
| SIEM | Wazuh 4.x |
| Manager | Ubuntu Server |
| Endpoint | Windows 10 |
| Virtualization | VirtualBox |

---

# 🏗️ Lab Architecture

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
                 |   PowerShell Events  |
                 +----------------------+
```

---

# ⚙️ Test Scenario

1. Enable PowerShell logging.
2. Execute PowerShell commands.
3. Verify event collection in Wazuh.
4. Investigate the generated alerts.

---

# 🚨 Detection Results

- PowerShell execution detected
- Windows event collected
- Wazuh alert generated
- Event successfully investigated

---

# 📸 Screenshots

| Screenshot | Description |
|------------|-------------|
| Lab-Setup.png | Home Lab |
| PowerShell-Command.png | Executed PowerShell Command |
| Wazuh-Alert.png | Alert Generated |
| Alert-Details.png | Rule Details |
| Dashboard.png | Wazuh Dashboard |

---

# 📄 Incident Report

📄 **[Incident-Report.md](Incident-Report.md)**

---

# 📚 Documentation

📘 **[Documentation/PowerShell-Detection.md](Documentation/PowerShell-Detection.md)**

---

# 🧠 Skills Demonstrated

- Wazuh SIEM
- Windows Security
- PowerShell
- Log Analysis
- Threat Hunting
- Incident Investigation
- MITRE ATT&CK

---

# 🛡️ MITRE ATT&CK

**Technique:** T1059.001 – PowerShell

**Tactic:** Execution

---

# ✅ Project Outcome

Successfully detected and investigated PowerShell execution events using Wazuh SIEM, improving practical SOC monitoring and threat detection skills.

---

## 👨‍💻 Author

**Muhammad Tashfeen**

Cyber Security Student | Aspiring SOC Analyst
