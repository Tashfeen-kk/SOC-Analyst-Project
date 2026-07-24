# Incident Report – Windows Logon Failure Detection using Wazuh SIEM

## Incident Summary

Wazuh SIEM successfully detected multiple failed Windows logon attempts on the monitored Windows 10 endpoint. The events were collected from the Windows Security Log (Event ID 4625), allowing investigation of unsuccessful authentication attempts that may indicate brute-force or password guessing activity.

---

## Objective

To validate that Wazuh can detect failed Windows authentication events and generate alerts for security monitoring and incident investigation.

---

## Incident Information

| Field | Value |
|-------|-------|
| Incident Type | Failed Windows Logon |
| Detection Source | Windows Security Event Logs |
| Event ID | 4625 |
| Rule | Windows Logon Failure |
| Severity | Medium |
| Status | Detected |

---

## Lab Environment

- SIEM: Wazuh 4.x
- Manager: Ubuntu Server
- Endpoint: Windows 10
- Virtualization: VirtualBox

---

## Steps Performed

1. Connected the Windows 10 agent to Wazuh.
2. Verified Windows Security Event collection.
3. Entered an incorrect password multiple times.
4. Generated failed authentication events.
5. Confirmed alert generation in the Wazuh Dashboard.
6. Investigated the alert details.

---

## Investigation Findings

- Wazuh successfully collected Event ID 4625.
- Failed authentication attempts were detected in real time.
- Alert details included the username, event time, endpoint, and Windows security information.
- The activity matched a failed logon scenario suitable for SOC investigation.

---

## Impact Assessment

Repeated failed logon attempts may indicate:
- Brute-force attacks
- Password guessing attempts
- Unauthorized access attempts
- Misconfigured user credentials

Early detection helps SOC analysts investigate suspicious authentication activity before successful compromise.

---

## MITRE ATT&CK Mapping

**Tactic:** Credential Access

**Technique:** T1110 – Brute Force

---

## Recommendations

- Monitor repeated failed logon attempts.
- Enable account lockout policies.
- Review authentication logs regularly.
- Investigate repeated failures from the same user or source.
- Enforce strong password policies and multi-factor authentication (MFA).

---

## Conclusion

The Windows Logon Failure Detection project was successfully completed. Wazuh accurately detected failed authentication attempts and generated alerts for investigation, demonstrating how SIEM solutions help SOC analysts identify and respond to suspicious login activity.
