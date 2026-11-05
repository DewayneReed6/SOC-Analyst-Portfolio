# Project 003 — Suspicious Login Investigation

## Project Overview

In this simulated SOC investigation, I analyzed suspicious Windows authentication activity involving multiple failed login attempts followed by successful Remote Desktop Protocol (RDP) access.

My goal was to identify potential unauthorized access, investigate post-login activity, and recommend appropriate incident-response actions.

## Investigation Summary

| Category | Finding |
|---|---|
| Incident Type | Unauthorized RDP Access |
| Severity | High |
| Classification | True Positive |
| Affected Account | jsmith |
| Workstation | FINANCE-PC01 |
| Source IP | 203.0.113.45 (simulated) |

## Tools and Technologies

- Simulated SIEM environment
- Windows Security Event Logs
- Windows Event IDs 4624, 4625, and 4688
- RDP authentication analysis
- Incident-response procedures

## Key Findings

1. Five failed login attempts occurred before a successful login.
2. The successful login used RDP Logon Type 10.
3. The employee denied initiating the remote session.
4. IT confirmed the source was not an approved remote-access endpoint.
5. Suspicious command-line activity followed authentication.

## Incident Response

I recommended isolating the affected workstation, securing the account, terminating unauthorized access, preserving evidence, and investigating additional endpoint activity.

## Final Assessment

The evidence strongly supported unauthorized remote access and possible post-login reconnaissance.

There was insufficient evidence to confirm malware installation or data theft.

## Skills Demonstrated

- Security Alert Triage
- Windows Event Log Analysis
- Suspicious Login Investigation
- Incident Classification
- Incident Response
- Security Documentation

## Full Investigation Report

[View My Investigation Report](Investigation-Report.md)

---

**Training Disclaimer:** This investigation uses fictional event logs and a guided scenario for cybersecurity portfolio development.
