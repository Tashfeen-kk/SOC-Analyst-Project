# Incident Report – Brute Force Attack Detection using Wazuh SIEM

## Incident Summary

An authorized brute-force simulation was conducted against a Windows 10 endpoint in a controlled home lab. Wazuh SIEM collected Windows Security Event ID 4625 (Failed Logon) events and generated alerts, allowing investigation of repeated authentication failures.

---

## Objective

To validate Wazuh's ability to detect repeated failed authentication attempts that may indicate a brute-force attack.

---

## Incident Information

| Field | Value |
|-------|-------|
| Incident Type | Brute Force Attack |
| Detection Source | Windows Security Logs |
| Event ID | 4625 |
| SIEM | Wazuh |
| Status | Detected |

---

## Lab Environment

- Ubuntu Server
- Wazuh SIEM
- Windows 10
- Kali Linux
- VirtualBox

---

## Steps Performed

1. Verified Wazuh agent connectivity.
2. Performed an authorized brute-force simulation.
3. Generated multiple failed login attempts.
4. Observed Event ID 4625 in Windows Security Logs.
5. Investigated alerts in the Wazuh Dashboard.

---

## Investigation Findings

- Multiple failed login attempts detected.
- Authentication alerts generated.
- Source IP identified.
- Timeline confirmed repeated login failures.

---

## Impact Assessment

Repeated failed authentication attempts may indicate password guessing or brute-force activity. Early detection enables SOC analysts to investigate and respond before unauthorized access is achieved.

---

## MITRE ATT&CK Mapping

Tactic: Credential Access

Technique: T1110 – Brute Force

---

## Recommendations

- Enable account lockout policies.
- Use multi-factor authentication (MFA).
- Monitor repeated authentication failures.
- Investigate unknown source IP addresses.
- Enforce strong password policies.

---

## Conclusion

The project successfully demonstrated Wazuh's capability to detect and investigate repeated failed login attempts in a controlled SOC lab.
