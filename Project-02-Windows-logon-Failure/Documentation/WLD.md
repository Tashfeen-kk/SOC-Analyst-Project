# Windows Logon Failure Detection Documentation

## Purpose

The purpose of this project is to detect failed Windows login attempts using Wazuh SIEM and Windows Security Event Logs.

---

## Technologies Used

- Wazuh SIEM
- Ubuntu Server
- Windows 10
- VirtualBox

---

## Configuration

### Step 1
Install Wazuh Manager.

### Step 2
Connect the Windows Agent.

### Step 3
Verify Security Event Log collection.

### Step 4
Confirm that Event ID 4625 is being collected.

---

## Test Procedure

1. Log in with an incorrect password.
2. Repeat the failed login several times.
3. Open the Wazuh Dashboard.
4. Search for Event ID 4625 or authentication alerts.
5. Review the generated alert.

---

## Detection

Wazuh generated alerts for failed Windows authentication attempts.

Relevant information included:
- Username
- Event ID
- Rule ID
- Timestamp
- Source endpoint

---

## MITRE ATT&CK

Technique:
- T1110 – Brute Force

Tactic:
- Credential Access

---

## Outcome

The project successfully demonstrated how Wazuh can detect failed Windows login attempts and support SOC analysts during authentication-related investigations.
