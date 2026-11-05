# Project 003 — Suspicious RDP Login Investigation

## 1. Executive Summary

During a simulated Security Operations Center (SOC) investigation, I analyzed multiple failed Windows authentication attempts followed by a successful Remote Desktop Protocol (RDP) login.

The affected account was `jsmith` on workstation `FINANCE-PC01`. Additional evidence strongly indicated unauthorized remote access, followed by suspicious command-line activity.

**Incident Classification:** True Positive  
**Severity:** High  
**Incident Type:** Suspected Account Compromise / Unauthorized Remote Access  
**Environment:** Simulated SOC Training Scenario  
**Investigation Status:** Initial investigation completed; full impact undetermined

## 2. Investigation Objectives

- Identify suspicious authentication patterns.
- Analyze Windows Security Event IDs.
- Determine whether remote access was authorized.
- Investigate activity following successful authentication.
- Recommend containment and further investigation.
- Document findings using evidence-based conclusions.

## 3. Tools and Technologies

- Simulated SIEM event logs
- Windows Security Event Logs
- Windows Event IDs 4624, 4625, and 4688
- RDP authentication analysis
- Incident-response methodology

## 4. Initial Security Alert

The SIEM generated an alert after detecting five failed authentication attempts followed by a successful login from the same source IP address.

| Field | Value |
|---|---|
| Username | `jsmith` |
| Hostname | `FINANCE-PC01` |
| Source IP | `203.0.113.45` |
| Authentication Type | RDP / RemoteInteractive |
| Logon Type | 10 |
| Failed Login Event | 4625 |
| Successful Login Event | 4624 |

The source IP is a reserved documentation address used exclusively for this simulation.

## 5. Incident Timeline

| Time | Event ID | Finding |
|---|---|---|
| 09:15:01 | 4625 | Failed login |
| 09:15:04 | 4625 | Failed login |
| 09:15:07 | 4625 | Failed login |
| 09:15:10 | 4625 | Failed login |
| 09:15:13 | 4625 | Failed login |
| 09:15:16 | 4624 | Successful RDP login |
| 09:16:02 | 4688 | `cmd.exe` executed |
| 09:16:18 | 4688 | `whoami.exe` executed |
| 09:16:35 | 4688 | `net.exe` executed |
| 09:17:10 | 4688 | `powershell.exe` executed |

## 6. Investigation Findings

### Finding 1 — Suspicious Authentication Pattern

Five failed login attempts occurred within approximately 12 seconds, followed by successful authentication three seconds later.

This pattern raised concern about possible password guessing or credential misuse.

### Finding 2 — Unauthorized Remote Access

The successful authentication used Logon Type 10, indicating remote interactive access.

In the simulation, the employee denied initiating the session, and IT confirmed that the source IP was not associated with an approved remote-access endpoint.

These findings strongly supported suspected unauthorized access.

### Finding 3 — Suspicious Post-Login Activity

Shortly after authentication, the workstation recorded execution of several Windows command-line tools:

- `cmd.exe`
- `whoami.exe`
- `net.exe`
- `powershell.exe`

These tools have legitimate administrative uses. However, their execution following suspected unauthorized access warranted further investigation.

The available evidence suggested possible reconnaissance, but the precise commands and their results were not provided.

## 7. Incident Classification

**Classification: True Positive**

The alert represented a genuine security concern supported by authentication logs, employee confirmation, and IT validation.

**Confirmed or strongly supported:**
- Repeated failed authentication attempts
- Successful remote interactive login
- Employee denial of the session
- Unapproved source IP
- Subsequent process execution

**Not established:**
- Malware installation
- Data exfiltration
- Privilege escalation
- Lateral movement
- Full scope of account compromise

## 8. Containment and Response

In the simulation, the incident-response team contained the affected workstation and secured the user account.

My recommended response included:

1. Escalating the incident to the appropriate response team.
2. Isolating the affected endpoint under the incident-response playbook.
3. Revoking unauthorized remote sessions.
4. Securing the affected user account and credentials.
5. Preserving authentication and endpoint evidence.
6. Reviewing additional process, file-access, and network logs.
7. Validating the system before restoring normal access.

## 9. Recommended Security Improvements

- Enforce multifactor authentication for remote access.
- Restrict RDP access to approved pathways.
- Implement appropriate account lockout and rate-limiting controls.
- Monitor failed-to-successful authentication sequences.
- Alert on unusual remote logins and suspicious process activity.
- Review privileged account access and endpoint security controls.

## 10. Final Assessment

The investigation identified a suspicious authentication sequence involving five failed login attempts followed by successful RDP access.

Employee and IT confirmation strongly supported unauthorized access. Subsequent process creation events raised additional concern about possible reconnaissance.

The incident was classified as a true positive requiring containment and further forensic investigation.

There was insufficient evidence to conclude that malware was installed or sensitive information was stolen.

## 11. Skills Demonstrated

- SOC Alert Triage
- Windows Security Event Analysis
- RDP Authentication Investigation
- Security Log Correlation
- Incident Classification
- Threat Containment Recommendations
- Evidence-Based Reporting
- Incident Documentation

---

**Portfolio Note:** This project is based entirely on fictional security logs and a guided SOC training scenario. It does not represent an investigation of a real organization or production system.
