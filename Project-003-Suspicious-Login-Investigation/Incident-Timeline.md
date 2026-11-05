# Incident Timeline — Suspicious RDP Login

**Incident:** #003  
**Severity:** High  
**Environment:** Simulated SOC Investigation

## Event Timeline

| Time | Event | Security Significance |
|---|---|---|
| 09:15:01–09:15:13 | Five failed logins | Possible password guessing |
| 09:15:16 | Successful RDP login | Suspected unauthorized access |
| 09:16:02 | cmd.exe executed | Command-line activity |
| 09:16:18 | whoami.exe executed | Possible user enumeration |
| 09:16:35 | net.exe executed | Possible system reconnaissance |
| 09:17:10 | powershell.exe executed | Further investigation required |

## Analyst Assessment

The timeline shows a suspicious authentication sequence followed by command-line activity. Employee and IT confirmation strongly support unauthorized access.

The available evidence does not establish malware installation or data exfiltration.

**Classification:** True Positive

*All events are fictional and provided for training purposes.*
