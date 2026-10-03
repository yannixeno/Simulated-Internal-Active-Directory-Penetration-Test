# Simulated Internal Active Directory Penetration Test

An authorized penetration test of a simulated enterprise Windows and Active Directory environment.

## Penetration Test Report

This assessment documents the complete attack path from initial reconnaissance to domain compromise, including:

- Network and service enumeration
- MS17-010 EternalBlue exploitation
- SMB and Windows host compromise
- Password spraying
- Kerberoasting
- Offline password cracking
- Privilege escalation
- Active Directory enumeration
- BloodHound attack-path analysis
- Lateral movement through RDP
- Domain Administrator compromise
- Technical findings and remediation recommendations

### Read the Full Report

[**Open the Penetration Test Report →**](./Penetration%20Test.pdf)

## Project Summary

This project simulates an internal penetration test against a small enterprise Windows network containing multiple endpoints and Active Directory domain controllers.

The assessment followed a structured penetration testing methodology:

1. Information gathering and reconnaissance
2. Service and vulnerability enumeration
3. Initial access
4. Credential attacks
5. Privilege escalation
6. Post-exploitation
7. Lateral movement
8. Active Directory compromise
9. Findings documentation and remediation

The assessment demonstrated how outdated systems, legacy SMB services, weak service-account passwords, insufficient authentication controls, and excessive administrative privileges can be chained together to compromise an entire Windows domain.

## Tools Used

- Nmap
- Metasploit Framework
- Meterpreter
- Impacket
- Hashcat
- BloodHound
- xfreerdp
- PowerShell
- SMB enumeration tools
- Active Directory and Kerberos attack techniques

## Key Findings

The assessment identified several high-impact attack paths, including:

- Remote code execution through MS17-010 EternalBlue
- Password spraying against exposed services
- Kerberoasting of service accounts
- Recovery of weak service-account credentials
- Lateral movement between domain systems
- Unauthorized privileged account creation
- Domain-level administrative compromise

## Remediation Focus

Recommended defensive improvements included:

- Applying missing security patches
- Disabling SMBv1
- Enforcing stronger password and account-lockout policies
- Implementing MFA for privileged accounts
- Auditing service accounts and SPNs
- Using Group Managed Service Accounts
- Restricting administrative RDP access
- Monitoring privileged group membership
- Improving network segmentation and detection capabilities

## Disclaimer

This project was completed in an authorized, simulated laboratory environment for educational and portfolio purposes. The techniques documented here should only be used against systems for which explicit permission has been obtained.
