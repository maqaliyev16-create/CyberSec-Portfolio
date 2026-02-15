# Lab Name: Linux Enumeration Challenge
**Certification:** eJPT  
**Date:** 2026-02-16

## Objective
Enumerate a Linux machine to identify services, users, and potential vulnerabilities.

## Tools
- Nmap
- Netcat
- Linux terminal commands (ls, cat, whoami, id, etc.)

## Steps Taken / Methodology
1. Ran `nmap -sV -p- target_ip` to identify open ports and services.
2. Enumerated users and groups using `cat /etc/passwd`.
3. Checked for sudo permissions and potential privilege escalation vectors.
4. Explored files in /home directory for sensitive info.
5. Documented findings with screenshots.

## Vulnerabilities Found
- Open SSH port with default user accounts
- Weak sudo permissions on user account

## Exploit / Proof of Concept
- Gained limited shell access using discovered credentials.

## Mitigation / Recommendations
- Enforce strong password policies
- Restrict sudo permissions
- Disable unused services

## Screenshots
- /screenshots/linux_enum1.png
- /screenshots/linux_enum2.png

## Lessons Learned
- Linux enumeration is the foundation of pentesting.
- Always check for privilege escalation vectors after initial access.
