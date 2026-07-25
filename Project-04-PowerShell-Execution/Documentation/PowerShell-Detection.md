# PowerShell Execution Detection Documentation

## Purpose

Demonstrate how Wazuh SIEM monitors and detects PowerShell execution events on a Windows endpoint.

---

## Technologies Used

- Wazuh SIEM
- Ubuntu Server
- Windows 10
- PowerShell
- VirtualBox

---

## Test Procedure

1. Verify the Wazuh Agent is connected.
2. Enable PowerShell logging.
3. Execute one or more PowerShell commands.
4. Confirm that the events appear in Wazuh.
5. Review the generated alerts.

---

## Detection

- PowerShell execution detected
- Event collected by Wazuh
- Alert generated for investigation

---

## Skills Learned

- Wazuh SIEM
- Windows Event Logging
- PowerShell Monitoring
- Threat Hunting
- Incident Investigation

---

## Outcome

The project confirmed that Wazuh can successfully collect and analyze PowerShell execution events, helping SOC analysts detect potentially suspicious command execution.
