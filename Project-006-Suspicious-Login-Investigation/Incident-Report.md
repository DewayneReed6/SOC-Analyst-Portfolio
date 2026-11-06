# Project 006 — SOC Incident Investigation Report

## 1. Incident Overview

**Incident Type:** Suspicious Remote Login / Potential Account Compromise

**Date:** November 5, 2026

**Affected Host:** FINANCE-PC01

**Affected Account:** jsmith

**Source IP:** 203.0.113.45

**Classification:** Suspicious Activity — Needs Further Investigation

**Severity:** Medium (Provisional)

**Status:** Investigation Pending

## 2. Executive Summary

During a simulated security investigation, multiple failed authentication attempts were identified against the jsmith account.

Five failed remote login attempts were followed by one successful remote interactive login from the same source IP address.

Shortly afterward, several Windows command-line utilities were executed on the affected workstation.

The activity may indicate password guessing and post-login reconnaissance. However, the available evidence does not confirm unauthorized access or establish that the remote session launched the processes.

## 3. Evidence Collected

### Authentication Events

- Event ID 4625: Failed login
- Event ID 4624: Successful login
- Source IP: 203.0.113.45
- Target Account: jsmith
- Logon Type: 10 (Remote Interactive)
- Failed Attempts from Source IP: 5
- Successful Login: 08:15:45

### Process Creation Events

Windows Event ID 4688 recorded the following processes on FINANCE-PC01:

- 08:16:10 — cmd.exe
- 08:16:20 — whoami.exe
- 08:16:30 — net.exe

These processes can be legitimate administrative tools but may also be used during system reconnaissance.

## 4. Investigation Findings

The authentication events show repeated failed login attempts followed by a successful remote login.

The process events show command-line activity on the same workstation within approximately one minute of the successful authentication.

The sequence is suspicious but does not prove malicious activity.

## 5. Risk Assessment

**Provisional Severity: Medium**

Potential risks include:

- Unauthorized account access
- Credential guessing
- Account enumeration
- Internal system reconnaissance

Severity should be reassessed if additional evidence confirms compromise, elevated privileges, or broader impact.

## 6. Recommended Response Actions

1. Verify the remote login with the account owner.
2. Review RDP session and authentication records.
3. Collect complete process command lines and process IDs.
4. Correlate process events with the authenticated logon session.
5. Review endpoint security alerts and related activity.
6. Escalate to a senior analyst for validation and response decisions.
7. If compromise is confirmed, follow approved account containment and credential reset procedures.

## 7. Final Assessment

The available logs support a finding of suspicious authentication and process activity.

The incident remains classified as Suspicious Activity — Needs Further Investigation.

Account compromise has not been confirmed.

## 8. Skills Demonstrated

- Windows Security Event Analysis
- Authentication Log Investigation
- Process Creation Analysis
- Timeline Reconstruction
- Incident Classification
- Risk Assessment
- SOC Incident Documentation

## Disclaimer

This is a simulated SOC investigation created for cybersecurity training and portfolio development. All events, users, hosts, and IP addresses are fictional.

