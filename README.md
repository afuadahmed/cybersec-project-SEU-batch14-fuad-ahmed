# Vulnerability Assessment and Penetration Testing (VAPT)

A hands-on cybersecurity project demonstrating the Vulnerability Assessment and Penetration Testing (VAPT) process in a controlled lab environment using **Kali Linux**, **Metasploitable 2**, **Nessus**, and **Metasploit Framework**.

The project covers vulnerability scanning, analysis of security findings, exploitation of an intentionally vulnerable system, and basic post-exploitation verification.

## Project Overview

The objective of this project was to gain practical experience with the VAPT lifecycle by assessing an intentionally vulnerable Metasploitable 2 machine in an isolated lab environment.

The assessment included:

- Configuring a vulnerability scan against the target system
- Performing vulnerability assessment using Nessus
- Reviewing and analyzing discovered vulnerabilities
- Examining vulnerabilities based on severity and technical details
- Validating selected vulnerabilities through controlled exploitation
- Obtaining shell access to the vulnerable machine
- Performing basic post-exploitation verification
- Documenting the assessment with screenshots and findings

## Lab Environment

| Component | Purpose |
|---|---|
| Kali Linux | Penetration testing / attacker machine |
| Metasploitable 2 | Intentionally vulnerable target machine |
| Nessus Essentials | Vulnerability scanning and assessment |
| Metasploit Framework | Controlled exploitation and validation |
| VMware | Virtualized and isolated lab environment |

## Vulnerability Assessment

A **Basic Network Scan** was configured in Nessus against the Metasploitable 2 target.

The scan identified vulnerabilities across multiple severity levels, including critical, high, medium, low, and informational findings.

The findings were reviewed to understand:

- Vulnerability severity
- Affected services
- Technical descriptions
- Risk information
- CVSS information
- Recommended remediation
- Potential security impact

### Example Findings

Some of the findings investigated during the assessment included:

**Bind Shell Backdoor Detection**

Nessus detected a critical backdoor-related vulnerability that could potentially allow unauthorized command execution on the vulnerable system.

**SSL DROWN Attack Vulnerability**

The scan also identified SSL/TLS-related weaknesses, including exposure associated with obsolete or weakened cryptographic configurations.

These findings demonstrated how automated vulnerability scanners can help identify and prioritize weaknesses before further manual validation.

## Penetration Testing

Following the vulnerability assessment, selected weaknesses were investigated in the controlled lab environment using the **Metasploit Framework**.

The testing demonstrated how a vulnerability discovered during an assessment can potentially be validated through controlled exploitation.

A Metasploit session was successfully established against the intentionally vulnerable Metasploitable 2 system.

## Post-Exploitation Verification

After obtaining access to the lab target, basic commands were executed to verify the level of access and gather system information.

Examples included:

- `whoami`
- `uname -a`
- `ifconfig`

The results demonstrated successful access to the vulnerable machine and provided information about the compromised environment.

## VAPT Workflow

The project followed the general workflow:

1. **Lab Setup**
2. **Target Identification**
3. **Vulnerability Scanning**
4. **Vulnerability Analysis**
5. **Risk Assessment**
6. **Controlled Exploitation**
7. **Post-Exploitation Verification**
8. **Documentation**

## Screenshots

Evidence from the assessment is available in the `screenshots/` directory.

The screenshots include:

- Nessus scan configuration
- Vulnerability scan summary
- Critical vulnerability findings
- Medium-severity vulnerability findings
- Exploitation results
- Post-exploitation command output

## Skills Demonstrated

- Vulnerability Assessment
- Penetration Testing Fundamentals
- Vulnerability Analysis
- Network Security
- Nessus Vulnerability Scanning
- Metasploit Framework
- Kali Linux
- Linux Command Line
- Security Testing Methodology
- Technical Documentation

## Key Learning Outcomes

Through this project, I gained practical experience in:

- Setting up an isolated penetration-testing laboratory
- Conducting vulnerability scans against a test system
- Interpreting vulnerability scanner results
- Understanding vulnerability severity and CVSS information
- Investigating security weaknesses
- Validating vulnerabilities through controlled exploitation
- Working with Metasploit sessions
- Performing basic post-exploitation verification
- Documenting security assessment results

## Ethical Notice

This project was performed entirely within an **authorized and controlled laboratory environment** using Metasploitable 2, an intentionally vulnerable system designed for cybersecurity training.

The techniques demonstrated in this repository are intended strictly for educational purposes and authorized security testing.

## Disclaimer

Always obtain explicit authorization before performing vulnerability scanning, penetration testing, or exploitation against systems or networks that you do not own or have permission to test.