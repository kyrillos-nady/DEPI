# Lord of The Root

## Overview
This repository documents the penetration testing steps conducted during the **Digital Egypt Pioneer Institute (DEPI)** project on web and network security. The project, titled **"Lord of The Root"**, involved reconnaissance, exploiting vulnerabilities, and privilege escalation to achieve root-level access on the target system.

### Team Members
- **Kyrillos Nady**
- Ahmed Ramdan
- Peter Issac

**Supervisor**: Eng. Ahmed Ashraf

---

## Contents

1. **Reconnaissance**  
   Identifying target IP, service enumeration using `nmap` and `zenmap`, port knocking, and discovering hidden resources.

2. **Initial Foothold**  
   Exploiting vulnerabilities via SQL injection and gaining access through compromised credentials.

3. **Privilege Escalation**  
   Leveraging kernel exploits to escalate privileges and retrieve the final flag.

---

## Key Highlights

### Reconnaissance
- Conducted an **nmap** scan to identify live hosts and open ports.
- Found an SSH port (22) and hints about port knocking. After triggering the sequence, discovered an Apache web server running on port 1337.

### Exploitation
- Located sensitive paths via Base64 decoding.
- Utilized **SQLMap** to uncover SQL injection vulnerabilities and extract database credentials.
- Successfully logged into the system using compromised credentials.

### Privilege Escalation
- Identified a kernel vulnerability on Ubuntu 14 using **searchsploit**.
- Compiled and executed a privilege escalation exploit to gain root access.
- Retrieved the root flag from `/root/Flag.txt`.

---

## Tools & Techniques
- **nmap**, **zenmap**
- **SQLMap**
- **Base64 decoding**
- **searchsploit**, **exploit-db**
- **gcc** for compiling privilege escalation exploits

---

## The Final Flag
> *“There is only one Lord of the Ring, only one who can bend it to his will. And he does not share power.” – Gandalf*

---
