# Small Company Security Design

 ## Project Overview

This project demonstrates a basic security architecture for a imaginary small company. The objective is to identify valuable assets, analyze common cyber threats, and recommend practical security controls.

# Company Overview
Company Name: ABC Solutions

## Environment

- 50 Employees
- Windows Server
- Employee Laptops (Windows 11)
- Database Server
- Microsoft 365
- Office Wi-Fi
- Cloud Storage

# Assets

- Employee laptops
- Windows Server
- Database Server
- Microsoft 365
- Cloud Storage
- Office Network
-Or anything other valuable to the company

# Threats Identified
- Phishing
- Malware
- Ransomware
- Password Attacks
- Insider Threat
- Device Theft

# Security Controls
## Identity Security
- Multi-Factor Authentication (MFA)
- Strong Password Policy
- Role-Based Access Control (RBAC)
- Least Privilege

## Network Security
- Firewall
- Secure Wi-Fi
- VPN for Remote Access
- Network Segmentation

## Endpoint Security
- Antivirus
- Endpoint Detection and Response (EDR)
- Automatic Updates

## Data Security
- HTTPS/TLS
- Full Disk Encryption(BitLocker)
- Regular Backups

## Monitoring
- Logging
- Security Information and Event Management (SIEM)

# Example Attack:

## Phishing Attack

An employee enters their Microsoft 365 credentials into a fake login page.

### Impact
- Account compromise
- Unauthorized access
- Potential data theft

### Mitigation
- MFA
- Email Security
- Security Awareness Training
- Conditional Access
- Login Monitoring

# Security Architecture

   Internet

   Firewall
   
   Office Network

   Windows Server

   Employee Devices

   Database

   Cloud Storage

Security controls are applied throughout including MFA, EDR, logging, encryption, and backups.

# Key Security Principles
- Defense in Depth
- Zero Trust
- Least Privilege
- CIA Triad
- Identity and Access Management
- Encryption

# Lessons Learned
Through this project I learned how to:
- Identify organizational assets
- Analyze cyber threats
- Select appropriate security controls
- Apply Defense in Depth
- Understand the roles of SOC Analysts and Security Engineers
- Design a simple security architecture

# Future Improvements
- Data Loss Prevention (DLP)
- Privileged Access Management (PAM)
- Vulnerability Scanning
- Cloud Security
- Security Awareness Program
