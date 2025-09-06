# SOC Lab: Suricata + ELK Stack

This project is a hands-on Security Operations Center (SOC) lab that demonstrates intrusion detection and log visualization using **Suricata IDS** and the **ELK Stack (Elasticsearch, Logstash, Kibana)**.

 🔹 Lab Setup
- Attacker VM: Kali Linux
- Victim VM: Metasploitable
- IDS VM: Kali Linux running Suricata with custom detection rules
- ELK Stack: Elasticsearch, Logstash, Kibana
- Filebeat: Forwarding Suricata logs into Elasticsearch

All attacker → victim traffic was routed through the IDS VM.

 🔹 Features
- Custom Suricata rules for:
  - Reconnaissance (ICMP scans, Nmap, HTTP scans)
  - Exploitation (SQLi, XSS, EternalBlue, Command Injection)
  - Brute Force (SSH, RDP)
  - Phishing and Malware C2
  - Data Exfiltration
  - Ransomware activity
- Logs ingested with Filebeat into Elasticsearch
- Kibana dashboards for:
  - Source/destination IP analysis
  - Attack category distribution
  - Timeline of alerts

 🔹 Screenshots
 Sample dashboards and alerts can be found in `docs/screenshots/`.

 🔹 Report
A full project report is available in `docs/Project_Report.pdf`.

 🔹 Usage
1. Set up Suricata with the `custom.rules` file from this repo.
2. Configure Filebeat to forward Suricata EVE JSON logs into Elasticsearch.
3. Use Kibana to visualize alerts and investigate threats.

---

### Tags
`#CyberSecurity` `#Suricata` `#ELK` `#SIEM` `#Kibana` `#IDS`
