# 🌐 Project 05 – Nmap Network Scan Detection using Wazuh SIEM

> Detecting network reconnaissance activities using Nmap and monitoring security events with Wazuh SIEM.

---

# 📌 Project Overview

This project demonstrates how Wazuh SIEM can be used to monitor and investigate security events generated during an authorized Nmap network scan. Network reconnaissance is often the first phase of an attack, making early detection valuable for SOC analysts.

---

# 🎯 Objectives

- Perform an authorized Nmap scan against a Windows endpoint.
- Monitor security events generated during the scan.
- Investigate alerts using the Wazuh Dashboard.
- Understand how reconnaissance activity appears in security logs.
- Document the investigation process.

---

# 🖥️ Lab Environment

| Component | Technology |
|-----------|------------|
| SIEM | Wazuh 4.x |
| Attacker | Kali Linux |
| Target | Windows 10 |
| Manager | Ubuntu Server |
| Virtualization | VirtualBox |

---

# 🏗️ Lab Architecture

```text
             +----------------------+
             |     Kali Linux       |
             |      Nmap Scan       |
             +----------+-----------+
                        |
                        | Network Scan
                        |
             +----------v-----------+
             |     Windows 10       |
             |    Wazuh Agent       |
             +----------+-----------+
                        |
                        | Security Events
                        |
             +----------v-----------+
             |    Ubuntu Server     |
             |    Wazuh Manager     |
             +----------+-----------+
                        |
                        |
             +----------v-----------+
             |   Wazuh Dashboard    |
             +----------------------+
```

---

# ⚙️ Test Scenario

1. Verify Wazuh Agent connectivity.
2. Start an authorized Nmap scan from Kali Linux.
3. Monitor Windows security events.
4. Review generated alerts in Wazuh.
5. Investigate alert details.

---

# 🚨 Detection Results

- Security events collected
- Wazuh alerts generated
- Reconnaissance activity investigated
- Event timeline reviewed

---

# 📸 Screenshots

| Screenshot | Description |
|------------|-------------|
| Lab-Setup.png | Home Lab Topology |
| Kali-Nmap-Scan.png | Executed Nmap Scan |
| Wazuh-Alert.png | Wazuh Alert |
| Alert-Details.png | Alert Details |
| Dashboard.png | Wazuh Dashboard |
| Threat-Hunting.png | Threat Hunting View |

---

# 📄 Incident Report

📄 **[Incident-Report.md](Incident-Report.md)**

---

# 📚 Documentation

📘 **[Documentation/Nmap-Detection.md](Documentation/Nmap-Detection.md)**

---

# 🧠 Skills Demonstrated

- Wazuh SIEM
- Nmap
- Threat Hunting
- Windows Security
- Log Analysis
- Incident Investigation
- Network Monitoring

---

# ✅ Project Outcome

Successfully performed an authorized Nmap scan, collected related security events, and investigated the activity using Wazuh SIEM to strengthen practical SOC Analyst skills.

---

## 👨‍💻 Author

**Muhammad Tashfeen**

Cyber Security Student | Aspiring SOC Analyst
