# Lab: Packet Capture & Traffic Analysis

**Tools:** Wireshark, FTP/SFTP, SSH, wireless (WLAN) configuration

## What I did
- Captured traffic while sending ICMP, FTP, SFTP and SSH sessions, then took the captures apart in Wireshark.
- Showed the difference between **plaintext and encrypted protocols**. FTP exposed its data and the passive port it negotiated in the packet details. SSH and SFTP payloads were unreadable, and I could see the SSHv2 cipher and MAC selections in the handshake.
- Joined a lab Wi-Fi network, captured its traffic, then **turned on WLAN encryption** on the access point and confirmed the traffic was no longer readable.
- In the challenge section, generated malicious wireless traffic and analyzed it in Wireshark, filtering by BSSID and station.

## Takeaway
Seeing credentials and file contents in a raw capture makes it obvious why legacy protocols like FTP and Telnet should be replaced with SFTP and SSH, and why open Wi-Fi is a risk.
