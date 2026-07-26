# Brute Force Attack Detection Documentation

## Purpose

Demonstrate how Wazuh SIEM detects repeated failed Windows login attempts and supports SOC investigations.

---

## Technologies Used

- Wazuh SIEM
- Ubuntu Server
- Windows 10
- Kali Linux
- VirtualBox

---

## Test Procedure

1. Verify the Wazuh agent is connected.
2. Perform an authorized brute-force simulation.
3. Generate multiple failed login attempts.
4. Confirm Event ID 4625 collection.
5. Review alerts in the Wazuh Dashboard.

---

## Detection

- Failed authentication events collected
- Event ID 4625 detected
- Authentication alerts generated
- Timeline reviewed

---

## Skills Learned

- Authentication Monitoring
- Wazuh SIEM
- Threat Hunting
- Log Analysis
- Incident Investigation

---

## Outcome

The project demonstrated how Wazuh SIEM can detect repeated failed login attempts and provide centralized visibility for authentication-related investigations.
