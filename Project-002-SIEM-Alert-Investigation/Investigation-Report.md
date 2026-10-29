# SOC Investigation Report
## Project 002: Suspicious Cryptocurrency Mining Activity

### 1. Investigation Overview

Role: Junior SOC Analyst (Training Lab)
Platform: TryHackMe
Investigation Type: Suspicious Process Execution
Status: Investigation Completed

### 2. Incident Summary

During a simulated SIEM investigation, a security
alert was triggered by suspicious process activity
on a Windows workstation.

The investigation focused on identifying the process,
the user responsible, and the affected computer.

### 3. Evidence Collected

- Suspicious Process: cudominer.exe
- Username: Chris
- Hostname: HR_02
- Windows Event ID: 4688
- Log Source: Windows Event Logs

### 4. Investigation Analysis

I reviewed security event logs to identify the
process responsible for triggering the alert.

Windows Event ID 4688 records process creation
activity when the appropriate auditing is enabled.

The suspicious process was identified as
cudominer.exe, which is associated with
cryptocurrency mining.

The event was associated with user Chris
on workstation HR_02.

The process warranted further investigation
to determine whether its execution was authorized.

### 5. Security Risk

Potential risks associated with unauthorized
cryptocurrency mining include:

- Excessive CPU and system resource usage
- Reduced workstation performance
- Unauthorized software execution
- Potential compromise of the affected endpoint

### 6. Recommended Response

1. Verify whether the mining software was authorized.
2. Review additional process execution logs.
3. Investigate the process origin and file hash.
4. Check for suspicious network connections.
5. Escalate confirmed unauthorized activity.
6. Contain the affected workstation if necessary.
7. Document findings and recommended actions.

### 7. Investigation Conclusion

The SIEM investigation identified a cryptocurrency
mining-related process executing on workstation HR_02.

The activity was suspicious and required further
validation to determine whether it was authorized.

This exercise demonstrated my ability to investigate
SIEM alerts, analyze Windows security events,
and document potential security incidents.

### 8. Skills Demonstrated

- SIEM Monitoring
- Security Alert Investigation
- Windows Event Log Analysis
- Suspicious Process Identification
- Incident Response Recommendations
- Security Documentation
