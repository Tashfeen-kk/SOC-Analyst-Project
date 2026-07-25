# Incident Report – Nmap Network Scan Detection using Wazuh SIEM

## Incident Summary

An authorized Nmap scan was performed from a Kali Linux system against a Windows 10 endpoint in a controlled home lab. Wazuh collected and displayed related security events, allowing analysis of reconnaissance activity.

---

## Objective

To validate that Wazuh can collect and present security events associated with network reconnaissance performed during an authorized Nmap scan.

---

## Incident Information

| Field | Value |
|-------|-------|
| Incident Type | Network Reconnaissance |
| Tool Used | Nmap |
| Detection Platform | Wazuh SIEM |
| Target | Windows 10 |
| Attacker | Kali Linux |
| Status | Investigated |

---

## Lab Environment

- Ubuntu Server (Wazuh Manager)
- Windows 10 (Agent)
- Kali Linux (Attacker)
- VirtualBox

---

## Steps Performed

1. Verified the Windows agent was connected.
2. Performed an authorized Nmap scan from Kali Linux.
3. Reviewed security events generated during the scan.
4. Investigated alerts in the Wazuh Dashboard.
5. Documented the findings.

---

## Investigation Findings

- Security events were successfully collected.
- Wazuh displayed relevant alerts for analysis.
- Event timestamps matched the scan activity.
- The collected information supported investigation of the reconnaissance phase.

---

## Impact Assessment

Reconnaissance activity can help defenders identify systems being probed before later stages of an attack. Monitoring these events improves visibility into suspicious network activity.

---

## Recommendations

- Continuously monitor reconnaissance-related events.
- Correlate network activity with endpoint security logs.
- Investigate repeated scans from the same source.
- Review firewall and endpoint logging configuration.
- Conduct regular threat hunting.

---

## Conclusion

The project successfully demonstrated how Wazuh SIEM can assist SOC analysts in investigating security events generated during an authorized Nmap network scan within a controlled lab environment.
