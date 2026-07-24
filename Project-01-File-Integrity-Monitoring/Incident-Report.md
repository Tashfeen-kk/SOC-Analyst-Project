Incident Report – File Integrity Monitoring using Wazuh

Incident Summary

Wazuh File Integrity Monitoring (FIM) successfully detected file creation, modification, and deletion events on the monitored Windows 10 endpoint. The alerts were generated in real time and displayed in the Wazuh dashboard for analysis.

Objective

To validate that Wazuh can monitor critical file system changes and generate alerts for unauthorized or suspicious modifications.

Lab Environment

SIEM: Wazuh
Operating System: Windows 10
Wazuh Server: Ubuntu Server
Virtualization: VirtualBox

Steps Performed

Configured File Integrity Monitoring (FIM) in Wazuh.
Connected the Windows agent to the Wazuh manager.
Created a test file.
Modified the file.
Deleted the file.
Verified that all events appeared in the Wazuh dashboard.

Observations

File creation was detected.
File modification was detected.
File deletion was detected.
Alerts included the file path, event time, agent name, and rule ID.

Impact

This demonstrates that Wazuh can detect unauthorized file changes, helping SOC analysts identify suspicious activity and maintain file integrity.

Conclusion

The File Integrity Monitoring project was successfully completed. Wazuh accurately monitored and reported file system changes, proving its effectiveness for security monitoring and incident investigation.
