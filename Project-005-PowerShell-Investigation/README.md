# Project 005 — Suspicious PowerShell Investigation

## Project Overview

This project demonstrates a simulated SOC
investigation involving suspicious Windows
PowerShell activity.

I analyzed Windows Event ID 4688 process
creation records using macOS Terminal.

## Investigation Scenario

A security alert identified Microsoft Word
launching PowerShell with an encoded command
on workstation FINANCE-PC01.

Additional processes included:

- whoami.exe
- cmd.exe
- net.exe

## Tools and Skills

- macOS Terminal
- grep and command-line log filtering
- Windows Event ID 4688 analysis
- Parent-child process investigation
- Incident timeline reconstruction
- Security alert triage
- Incident response documentation

## Key Findings

- PowerShell was launched by winword.exe.
- PowerShell used the -EncodedCommand option.
- Additional system utilities were launched.
- The suspicious process sequence lasted 15 seconds.
- Available evidence was insufficient to confirm
  malicious activity.

## Alert Classification

Needs Further Investigation

## Investigation Files

- [Windows Event Logs](windows-events.log)
- [Incident Timeline](Incident-Timeline.txt)
- [Alert Assessment](Alert-Assessment.md)
- [Incident Report](Incident-Report.md)

## Conclusion

This project demonstrates my ability to
investigate suspicious process activity,
analyze security logs, and document
incident response recommendations.

## Disclaimer

All logs and events are fictional and
used for cybersecurity training.
