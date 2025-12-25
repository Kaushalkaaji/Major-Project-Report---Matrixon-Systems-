# Major-Project-Report---Matrixon-Systems

Attack, Detection & Hardening of Enterprise Infrastructure Using SIEM

📌 Project Description

This project demonstrates a complete Red Team–Blue Team security workflow by simulating real-world cyberattacks on enterprise infrastructure, detecting security events using a SIEM solution (Wazuh), and applying effective system hardening measures. The goal is to understand how attacks occur, how they are detected, and how systems can be secured against them.

🎯 Objectives

    Simulate common cyberattacks on Linux servers
    
    Detect and analyze security events using Wazuh SIEM
    
    Correlate logs from multiple systems
    
    Implement system hardening techniques
    
    Compare security posture before and after hardening

🏗 Infrastructure Overview
The project uses a multi-VM architecture:

    Internal Server (Victim) – Target of attacks
    
    Web Server (Attacker & Victim) – Used for web-based attacks and log generation
    
    SIEM Server – Centralized log collection, correlation, and alerting

Logs from all servers are forwarded to the SIEM server for real-time monitoring and investigation.

🛠 Tools & Technologies Used

    Wazuh SIEM
    
    Linux (Ubuntu)
    
    Nmap, Hydra, Nikto, Gobuster
    
    Apache Web Server
    
    UFW Firewall
    
    Fail2Ban
    
    Auditd
    
    Virtual Machines (Azure)

Red Team Activities (Attack Simulation)

    Port scanning and service enumeration
    
    SSH brute-force attacks
    
    Web vulnerability scanning and directory enumeration
    
    Privilege escalation and system enumeration

🔵 SIEM Monitoring & Investigation

    Real-time log collection using Wazuh agents
    
    Detection of authentication failures, scans, and web attacks
    
    Alert generation and visualization through the SIEM dashboard
    
    Event correlation across multiple endpoints

🛡 Hardening & Mitigation

    SSH hardening (port change, disabling root login, limiting attempts)
    
    Firewall configuration using UFW
    
    Apache web server hardening
    
    Brute-force protection with Fail2Ban
    
    System auditing using Auditd

🔁 Re-Attack & Validation

    After hardening, the same attacks were re-executed to validate security improvements. Results showed reduced attack success, blocked brute-force attempts, and improved alert visibility.

Conclusion

    This project effectively demonstrates how enterprise infrastructure can be attacked, monitored, and secured using SIEM tools and security best practices, providing strong foundational experience in cybersecurity operations.
