# 🔐 Project 06 – Brute Force Attack Detection using Wazuh SIEM

> Detecting brute-force login attempts using Windows Security Logs and Wazuh SIEM.

---

# 📌 Project Overview

This project demonstrates how Wazuh SIEM detects repeated failed Windows authentication attempts that may indicate a brute-force attack. Authentication monitoring is a critical responsibility of SOC analysts for identifying unauthorized access attempts.

---

# 🎯 Objectives

- Simulate a brute-force login attack in a controlled lab.
- Monitor failed authentication events.
- Investigate alerts using Wazuh.
- Correlate multiple failed logins.
- Document the incident.

---

# 🖥️ Lab Environment

| Component | Technology |
|-----------|------------|
| SIEM | Wazuh 4.x |
| Manager | Ubuntu Server |
| Target | Windows 10 |
| Attacker | Kali Linux |
| Virtualization | VirtualBox |

---

# 🏗️ Lab Architecture

Kali Linux
      │
      │ Brute Force Attempts
      ▼
Windows 10 (Wazuh Agent)
      │
      ▼
Ubuntu Server (Wazuh Manager)
      │
      ▼
Wazuh Dashboard

---

# ⚙️ Test Scenario

1. Verify agent connectivity.
2. Launch an authorized brute-force simulation.
3. Generate multiple failed login attempts.
4. Monitor Wazuh alerts.
5. Investigate authentication events.

---

# 🚨 Detection Results

- Multiple failed login attempts detected
- Windows Event ID 4625 collected
- Authentication alerts generated
- Source IP identified
- Timeline reviewed

---

# 📸 Screenshots

- Lab-Setup.png
- Attack-Simulation.png
- Failed-Login-Alerts.png
- Alert-Details.png
- Dashboard.png
- Event-Viewer.png

---

# 📄 Incident Report

📄 Incident-Report.md

---

# 📚 Documentation

📘 Documentation/Brute-Force-Detection.md

---

# 🧠 Skills Demonstrated

- Wazuh SIEM
- Authentication Monitoring
- Windows Security
- Log Analysis
- Threat Hunting
- Incident Response
- MITRE ATT&CK

---

# 🛡️ MITRE ATT&CK

Technique: T1110 – Brute Force

Tactic: Credential Access

---

# ✅ Project Outcome

Successfully detected repeated failed login attempts using Wazuh SIEM and investigated authentication events in a controlled lab environment.

---

## 👨‍💻 Author

Muhammad Tashfeen

Cyber Security Student | Aspiring SOC Analyst
