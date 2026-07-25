# Incident Report – PowerShell Execution Detection using Wazuh SIEM

## Incident Summary

Wazuh SIEM successfully detected PowerShell execution events on the monitored Windows endpoint. The generated alerts provided visibility into command execution and demonstrated how SOC analysts can investigate PowerShell activity.

---

## Objective

To validate that Wazuh can detect PowerShell execution events and generate alerts for monitoring and incident investigation.

---

## Incident Information

| Field | Value |
|-------|-------|
| Incident Type | PowerShell Execution |
| Detection Source | Windows Event Logs |
| SIEM | Wazuh |
| Severity | Medium |
| Status | Detected |

---

## Lab Environment

- Wazuh SIEM
- Ubuntu Server
- Windows 10
- VirtualBox

---

## Steps Performed

1. Enabled PowerShell logging.
2. Executed PowerShell commands.
3. Verified event collection.
4. Investigated alerts in the Wazuh Dashboard.

---

## Investigation Findings

- PowerShell execution was successfully logged.
- Wazuh generated alerts in real time.
- Event details included timestamp, endpoint, user, and executed process.

---

## Impact Assessment

PowerShell is commonly used for system administration but is also abused by attackers for malicious activities. Monitoring PowerShell execution helps SOC analysts detect suspicious behavior early.

---

## MITRE ATT&CK Mapping

**Tactic:** Execution

**Technique:** T1059.001 – PowerShell

---

## Recommendations

- Enable PowerShell Script Block Logging.
- Investigate unexpected PowerShell activity.
- Correlate PowerShell events with other security logs.
- Apply the principle of least privilege.
- Regularly review Windows event logs.

---

## Conclusion

The project successfully demonstrated Wazuh's ability to detect and investigate PowerShell execution events, improving endpoint visibility and SOC monitoring capabilities.
