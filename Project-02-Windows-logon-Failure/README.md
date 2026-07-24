# 🔐 Project 02 – Windows Logon Failure Detection using Wazuh SIEM

> Detecting failed Windows logon attempts using Wazuh SIEM and Windows Security Event Logs.

---

# 📌 Project Overview

This project demonstrates how Wazuh SIEM detects failed Windows logon attempts by monitoring Windows Security Event Logs. Failed authentication events are important indicators of brute-force attacks, password guessing, or unauthorized access attempts.

---

# 🎯 Objectives

- Monitor failed Windows logon events.
- Generate real-time alerts in Wazuh.
- Investigate authentication failures.
- Analyze Windows Security Event Logs.
- Improve SOC investigation skills.

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
                 | Failed Logon Events  |
                 +----------------------+
```

---

# ⚙️ Configuration

- Installed Wazuh Manager.
- Connected Windows Agent.
- Enabled Windows Security Event monitoring.
- Verified event collection.

---

# 🧪 Test Scenario

1. Enter an incorrect password several times.
2. Generate failed logon events.
3. Verify alerts in the Wazuh Dashboard.
4. Review alert details and Event ID.

---

# 🚨 Detection Results

- Failed Windows Logon detected
- Event ID 4625 collected
- Authentication failure alert generated
- Alert mapped to MITRE ATT&CK

---

# 📸 Screenshots

Store all screenshots inside the **Screenshots/** folder.

| Screenshot | Description |
|------------|-------------|
| Lab-Setup.png | Home Lab |
| Failed-Login.png | Incorrect Password Attempt |
| Wazuh-Alert.png | Alert Generated |
| Alert-Details.png | Rule Details |
| Event-Details.png | Windows Security Event |
| Dashboard.png | Wazuh Dashboard |

---

# 📄 Incident Report

📄 **[Incident Report](Incident-Report.md)**

---

# 🧠 Skills Demonstrated

- Wazuh SIEM
- Windows Security Logs
- Authentication Monitoring
- Log Analysis
- Incident Investigation
- Threat Hunting

---

# 🛡️ MITRE ATT&CK

**Technique:** T1110 – Brute Force

**Tactic:** Credential Access

---

# ✅ Project Outcome

Successfully detected failed Windows logon attempts using Wazuh SIEM and analyzed authentication events for security monitoring and incident response.

---

# 👨‍💻 Author

**Muhammad Tashfeen**

Cyber Security Student | Aspiring SOC Analyst

GitHub: https://github.com/YOUR_USERNAME

LinkedIn: https://linkedin.com/in/YOUR_PROFILE
