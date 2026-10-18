# Lab: Security Monitoring & Logging

**Tools:** Windows Event Viewer, Snort IDS (on pfSense), Linux rsyslog, Tripwire

## What I did
- Found **failed logon attempts** in the Windows Security log and reviewed the event details.
- Turned on **Snort** on the LAN interface, set up pass lists, generated ICMP traffic, and confirmed the alerts showed up in the Snort log.
- Configured **rsyslog** on Linux, generated failed login attempts, and tracked them in the logs.
- Set up **Tripwire** file-integrity monitoring and read its object summary report to spot changed files.

## Takeaway
You can't respond to what you can't see. Authentication logs, network IDS alerts and file-integrity checks each catch different parts of an attack, so you want all three feeding a central log or SIEM.
