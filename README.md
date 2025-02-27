# vulnhub-box-walkthrough
This repository contains a list of vulnerable virtual machines from VulnHub that were used for penetration testing as part of this project.
Overview of cybersecurity & ethical hacking.
Purpose: To identify vulnerabilities and test security defenses using penetration testing techniques.
Vulnerable Machines Attempted

Pumpkin Garden CTF (Mission-Pumpkin v1.0) by Jayanth
Other machines attempted (if applicable).
Tools Used

Hardware: 4GB RAM (minimum), 20GB storage, Intel Dual Core CPU.
Software: Kali Linux, Nmap, Wireshark, Burp Suite, VirtualBox.
Implementation Summary (Walkthrough)

Network Scanning → Used nmap to identify open ports.
FTP Access → Anonymous login, retrieved note.txt for credentials.
HTTP Enumeration → Checked page source, found Base64-encoded credentials.
SSH Login → Used extracted credentials to log in as scarecrow.
Privilege Escalation → Used misconfigured sudo permissions to gain root access.
Final Flag Capture → Retrieved PumpkinGarden_Key and decoded it.
Findings & Recommendations

Successfully escalated privileges to root.
Identified security weaknesses in FTP, weak credentials, and misconfigured permissions.
Suggested stronger authentication, limiting open ports, and using encryption.
