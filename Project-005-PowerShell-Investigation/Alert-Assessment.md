# Project 005 — Security Alert Assessment

## Alert Information

Date: 2026-11-05
Host: FINANCE-PC01
User: jsmith
Windows Event ID: 4688

## Alert Classification

Status: Needs Further Investigation
Priority: Medium (Training Assessment)

## Evidence Observed

10:05:30 - winword.exe launched powershell.exe
10:05:35 - powershell.exe launched whoami.exe
10:05:40 - powershell.exe launched cmd.exe
10:05:45 - cmd.exe launched net.exe

The PowerShell command included -EncodedCommand.

## Analyst Findings

The process chain is suspicious because Microsoft
Word launched PowerShell with an encoded command,
followed by Windows system utilities.

These utilities can be used for legitimate
administration or attacker reconnaissance.

The available logs do not confirm malicious
execution, credential theft, or data exfiltration.

## Recommended Investigation

1. Obtain the full PowerShell command line.
2. Review endpoint detection alerts.
3. Check related network connections.
4. Verify whether the activity was authorized.
5. Preserve relevant logs and evidence.
6. Escalate according to incident response policy.

## Conclusion

The alert remains under investigation.
Additional evidence is required before a final
true-positive or false-positive determination.

## Training Disclaimer

All evidence is fictional and used for
cybersecurity training purposes.
