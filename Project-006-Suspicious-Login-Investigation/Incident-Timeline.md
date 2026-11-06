# Project 006 — Incident Timeline

## Investigation Details
- Incident Type: Suspicious Remote Login
- Affected Host: FINANCE-PC01
- Affected User: jsmith
- Source IP: 203.0.113.45
- Date: November 5, 2026
- Classification: Suspicious Activity — Needs Further Investigation

## Event Timeline

| Time | Event | Description |
|------|-------|-------------|
| 08:15:30 | 4625 | First failed login |
| 08:15:33 | 4625 | Second failed login |
| 08:15:36 | 4625 | Third failed login |
| 08:15:39 | 4625 | Fourth failed login |
| 08:15:42 | 4625 | Fifth failed login |
| 08:15:45 | 4624 | Successful remote interactive login |
| 08:16:10 | 4688 | cmd.exe executed |
| 08:16:20 | 4688 | whoami.exe executed |
| 08:16:30 | 4688 | net.exe executed |

## Initial Assessment

Five failed login attempts were followed by a successful
remote interactive login to the jsmith account.

Command-line processes were observed on the same host
shortly after the login.

The activity may indicate password guessing followed by
reconnaissance, but unauthorized access has not been confirmed.

## Recommended Next Steps

1. Verify whether jsmith initiated the remote login.
2. Review additional authentication and RDP session logs.
3. Examine process command lines and parent-child relationships.
4. Correlate process activity with the authenticated session.
5. Escalate to a senior analyst if suspicious activity is confirmed.


