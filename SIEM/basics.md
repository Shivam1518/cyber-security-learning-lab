# SIEM Basics

A SIEM (Security Information & Event Management) is a centralized platform that collects, normalizes, correlates, and analyzes security events from across an organization.

## 🔹 What SIEM Actually Does
- Collects logs from servers, endpoints, cloud, network devices, applications
- Normalizes data into a standard schema
- Correlates events to detect threats
- Alerts analysts with severity-based incidents
- Stores logs for auditing & investigations
- Builds dashboards for visibility
- Supports compliance (ISO, PCI-DSS, SOC2)

---

# 🔹 Core Components of a SIEM

## 1. **Collectors / Agents**
Gathers logs from:
- Firewall  
- EDR  
- Cloud (AWS, Azure, GCP)  
- Windows/Linux servers  
- Applications  
- Databases  

## 2. **Normalization Engine**
Converts different log formats → unified schema (fields like src_ip, dst_port, event_id).

Example:  
Different devices send different logs, SIEM makes them uniform.

## 3. **Correlation Engine**
The brain of SIEM.

Combines multiple events to detect:
- Brute force attacks  
- Privilege escalation  
- Lateral movement  
- Port scanning  
- Suspicious file activity  
- Command & control (C2) callbacks  

## 4. **Alerting System**
Generates alerts based on:
- Threshold rules  
- Pattern rules  
- Behavioral anomalies  
- MITRE ATT&CK mapping  

## 5. **Dashboard & Reporting**
Used by SOC analysts & management.

---

# 🔹 Log → Event → Alert → Incident (Flow)

1. **Raw Log**  
2. **Normalized Event**  
3. **Correlated Alert**  
4. **Incident**  
5. **Response Action**

---

# 🔹 Why SIEM Is Important
- Detects threats early  
- Gives complete visibility  
- Helps Incident Response (IR)  
- Reduces investigation time  
- Ensures compliance  
- Crucial for SOC operations  

---

# 🔹 SIEM vs SOAR  
(SOAR = automation layer)

| Feature | SIEM | SOAR |
|--------|------|------|
| Log collection | ✔ | ✘ |
| Correlation | ✔ | ✘ |
| Alerting | ✔ | ✔ |
| Automated response | Limited | ✔ |
| Playbooks | ✘ | ✔ |

They work together inside modern SOCs.

---

# 🔹 Common SIEM Use Cases

- Multiple failed logins → Success → Brute Force  
- New admin account created  
- Lateral movement (SMB, RDP)  
- Suspicious PowerShell commands  
- Data exfiltration spikes  
- Unexpected outbound connections  
- Malware execution patterns  

---

# 🔹 Tools to Explore Later
- Splunk  
- ELK / OpenSearch  
- Azure Sentinel  
- IBM QRadar  
- Seceon aiSIEM (your company uses this)  

---

This file gives full SIEM fundamentals to move forward with correlation and detection engineering.
