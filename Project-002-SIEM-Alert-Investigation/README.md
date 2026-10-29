# Project 002: SIEM Alert Investigation

## Project Overview
This project demonstrates my ability to investigate
suspicious security events using SIEM technology.

## Tools Used
- TryHackMe
- SIEM Training Environment
- Windows Event Logs

## Investigation Scenario
A security alert was triggered after a suspicious
process executed on a Windows workstation.

## Investigation Findings
- Suspicious Process: cudominer.exe
- Username: Chris
- Hostname: HR_02
- Windows Event ID: 4688
- Potential Threat: Cryptocurrency Mining

## Skills Demonstrated
- SIEM Alert Investigation
- Windows Event Log Analysis
- Suspicious Process Identification
- Security Event Correlation
- Incident Documentation

## Investigation Status
Training investigation completed.
Detailed incident report to follow.

## 9. Investigation Evidence

### Evidence 1: Suspicious Process Detection

![Suspicious Process](01-Suspicious-Process.png)

The SIEM dashboard identified cudominer.exe running
once in the simulated environment.

### Evidence 2: Process Execution Details

![Process Execution](02-Process-Execution-Details.png)

The event identified user Chris on workstation HR_02.
The executable path was C:\Users\Chris\temp\cudominer.exe.

### Evidence 3: Windows Security Event

![Windows Event 4688](03-Windows-Event-4688.png)

Windows Event ID 4688 provided process creation
evidence for the investigation.
