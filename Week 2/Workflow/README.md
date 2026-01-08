# Week 2 – SOC Lab Workflow

## Repository Structure
- Documentation → PDFs, notes, screenshots
- Workflow → Step-by-step commands and evidence
- Tickets → TheHive tickets, escalation emails
- Dashboards → Wazuh dashboard screenshots

## Workflow Steps
1. Alert Classification (Google Sheets)
2. Incident Classification (Docs)
3. Incident Response Lifecycle (Draw.io)
4. Wazuh Dashboard setup
5. TheHive Ticket creation
6. Evidence Preservation
7. Capstone Attack Simulation

# Alert & Incident Mapping

| Alert ID | Incident ID | Type            | CVSS | Priority  | Reason / Severity          | MITRE Technique | Description / Evidence             | Source IP      | Status    | Assigned To  | Date       | Hash / Notes            |
|----------|-------------|-----------------|------|-----------|----------------------------|-----------------|-----------------------------------|----------------|-----------|--------------|------------|-------------------------|
| 1        | INC-01      | Phishing        | 7.5  | High      | Suspicious email link      | T1566           | Phishing Email w/ malicious URL    | 10.0.0.5       | Closed    | SOC Analyst  | 01/06/2026 | Email headers checked   |
| 2        | INC-02      | SSH Brute Force | 5.3  | Medium    | No compromise              | T1110           | Multiple failed SSH logins         | 192.168.1.100  | Open      | Tier 1       | 01/06/2026 | Auth logs SHA256        |
| 3        | INC-03      | Log4Shell       | 9.8  | Critical  | RCE, public exploit        | T1190           | Exploit attempt detected           | 172.16.0.10    | Escalated | Tier 2       | 01/06/2026 | Wazuh alert evidence    |
| 4        | INC-04      | SQL Injection   | 8.2  | High      | Database compromise risk   | T1190           | Malicious query in logs            | 192.168.1.200  | Open      | SOC Analyst  | 01/06/2026 | DB logs hashed          |
| 5        | INC-05      | Malware Beacon  | 6.7  | Medium    | Suspicious outbound C2     | T1071           | Beacon traffic to known C2 IP      | 203.0.113.50   | Closed    | Tier 2       | 01/06/2026 | PCAP file SHA256        |
| 6        | INC-06      | Port Scan       | 3.0  | Low       | Reconnaissance only        | T1046           | Nmap scan detected                 | 198.51.100.25  | Closed    | Tier 1       | 01/06/2026 | Firewall logs           |
