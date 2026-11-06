# Project 006 — Suspicious Login & Account Compromise Investigation

## Project Overview
This project simulates a Security Operations Center (SOC) investigation involving repeated failed login attempts, a successful remote login, and suspicious process activity.

**Role:** Junior SOC Analyst  
**Environment:** Simulated Windows Security Logs  
**Tools:** macOS Terminal, grep, awk, Nano  
**Classification:** Suspicious Activity — Needs Further Investigation

## Investigation Objectives
- Identify failed and successful login attempts
- Investigate suspicious source IP addresses
- Analyze Windows Event IDs 4624, 4625, and 4688
- Correlate authentication and process activity
- Document findings and recommend next steps

## Key Findings
- Six failed logins were identified across the dataset.
- Five failed attempts originated from 203.0.113.45.
- The same IP subsequently recorded a successful remote login to jsmith.
- cmd.exe, whoami.exe, and net.exe ran on FINANCE-PC01 shortly afterward.
- The available evidence does not confirm account compromise.

## Incident Classification
Suspicious Activity — Needs Further Investigation

## Investigation Files
- [Security Events](security-events.log)
- [Incident Timeline](Incident-Timeline.md)
- [Incident Report](Incident-Report.md)

## Skills Demonstrated
- Security Log Analysis
- Windows Event ID Investigation
- Authentication Monitoring
- Process Activity Analysis
- Incident Documentation
- SOC Alert Triage

## Disclaimer
This project uses fictional security logs for educational and portfolio purposes. No real systems were compromised.


