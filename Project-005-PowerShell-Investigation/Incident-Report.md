# Project 005 — Suspicious PowerShell Investigation

## Incident Summary

Date: November 5, 2026
Host: FINANCE-PC01
User: jsmith
Event ID: 4688
Status: Needs Further Investigation
Priority: Medium (Training Assessment)

## Investigation Objective

Investigate suspicious PowerShell execution
and identify unusual process activity.

## Tools Used

- macOS Terminal
- grep
- Windows Event ID 4688 (Simulated)
- Process log analysis

## Incident Timeline

| Time | Process | Parent |
|------|---------|--------|
| 10:05:30 | powershell.exe | winword.exe |
| 10:05:35 | whoami.exe | powershell.exe |
| 10:05:40 | cmd.exe | powershell.exe |
| 10:05:45 | net.exe | cmd.exe |

## Investigation Findings

Microsoft Word launched PowerShell with
an encoded command.

PowerShell then launched whoami.exe and cmd.exe.

The cmd.exe process subsequently launched net.exe.

These events occurred within 15 seconds.

This activity may indicate suspicious script
execution or system discovery.

The available evidence does not confirm
malware infection or unauthorized access.

## Analyst Assessment

Classification: Needs Further Investigation

Additional evidence is required before
determining whether the alert is malicious.

## Recommended Actions

1. Preserve security logs.
2. Review the full PowerShell command.
3. Examine endpoint detection alerts.
4. Investigate related network activity.
5. Verify whether the activity was authorized.
6. Escalate according to incident response policy.

## Conclusion

This investigation demonstrates practical
SOC skills in Windows process log analysis,
incident triage, and security reporting.

## Training Disclaimer

All events are fictional and created
for hands-on cybersecurity training.
