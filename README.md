# Network Security Assessment

## Project Overview
This project is a hands-on network security assessment completed in an isolated cybersecurity home lab. I used Kali Linux and Nmap to identify open ports, examine network services, and document potential security risks on a Metasploitable 2 virtual machine.

## Project Objectives
- Identify open network ports and running services.
- Investigate potential security weaknesses.
- Practice using Nmap for network scanning.
- Document findings and recommend security improvements.

## Tools and Technologies
- Kali Linux
- Nmap
- Oracle VirtualBox
- Metasploitable 2

## Lab Environment
- Testing machine: Kali Linux
- Target machine: Metasploitable 2
- Target IP: 192.168.56.20 (private lab address)
- Network: Isolated VirtualBox internal network

## Security Findings

| Service | Port | Finding | Recommendation |
|---|---|---|---|
| FTP | 21 | Anonymous FTP login was allowed | Disable anonymous FTP access |
| Telnet | 23 | Telnet provides unencrypted communication | Replace Telnet with SSH |
| SSH | 22 | An outdated OpenSSH version was detected | Update SSH software |
| HTTP | 80 | An outdated Apache HTTP server was detected | Update the web server and apply patches |

Evidence and Reports
- [Full Security Assessment Report](report.txt)
- [Nmap Network Scan](nmap_scan.txt)
- [FTP Finding](ftp_finding.txt)
- [Telnet Finding](telnet_finding.txt)
- [SSH Finding](ssh_finding.txt)
- [HTTP Finding](http_finding.txt)
- [HTTP Security Headers Scan](http_headers.txt)

The HTTP security headers scan did not return header details, so no conclusion was made about missing headers.

## What I Learned
Through this project, I learned how to use Nmap to discover open ports, identify network services, interpret scan results, and write security findings with recommendations. This project strengthened my understanding of network security and vulnerability assessment.

## Ethical and Legal Notice
All testing was performed in an isolated, authorized home lab using an intentionally vulnerable Metasploitable 2 virtual machine. No external systems were tested.
