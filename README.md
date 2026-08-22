# -dawnsmithcyber
# 🛡️ Dawn Smith | SOC Analyst & Cybersecurity Researcher

Applying strong academic excellence in Financial Forensics to real-world cybersecurity challenges.

---

### Hi there, I'm Dawn 👋

I am a cybersecurity professional, Certified Fraud Examiner (CFE), and **Senior Researcher, Investigator, & Analyst Consultant** specializing in complex fraud and cyber investigations *(details protected under NDA)*. 

Alongside my investigative and consulting work, I serve as a Community Moderator for Gladys, where I lead **CompTIA Security+ SY0-701** study groups and teach practical **SOC Triage and Documentation**. I’m focused on hands-on security—investigating threats, finding weaknesses, and building stronger defenses against evolving attacks.

---

## 🛠️ Core Expertise & Focus
* **Threat Detection & Incident Response:** Triage, log analysis, and endpoint monitoring.
* **Fraud & Cyber Investigations:** Bridging financial crime analysis with technical controls.
* **Community Leadership:** Mentoring analysts, leading Security+ study groups, and teaching SOC workflows.

⚡ **Current Goal:** Continuously building and sharing hands-on labs to master the technical controls that drive organizational resilience.

---

## 🛠️ Technical Arsenal

### **Identity & Network Defense**
* **Firewalls & ACLs:** Configuring rules to enforce the Principle of Least Privilege.
* **MFA & IAM:** Strengthening authentication protocols to prevent unauthorized access.
* **VPN/TLS:** Securing data in transit across untrusted networks.
* **Microsoft Azure With Defender For Cloud:** Hands-on lab focused on cloud security posture management (CSPM) and workload protection, demonstrating how to deploy, configure, and monitor security within the Azure ecosystem to detect threats and remediate vulnerabilities in real-time.

### **Monitoring & Detection (The SOC Toolkit)**
* **SIEM (Splunk / ELK Stack):** Analyzing and parsing logs to identify anomalies, indicators of compromise, and upgrade/harden enterprise SIEM instances.
* **IDS/IPS:** Deploying **Snort / Suricata** to detect and block malicious traffic.
* **Endpoint Security:** Implementing **EDR / Sysmon** for granular visibility into host activity.

---

## 🚀 Featured Cybersecurity Labs & Projects

### Azure KQL: Moving from Reactive to Proactive Threat Hunting 🛡️
* **Project Overview:** Documents my transition from reactive security monitoring to proactive threat hunting using **Kusto Query Language (KQL)** within Azure Sentinel and Log Analytics to map attacker paths and create visual narratives.
* **Core Competencies:** Analyzing traffic flows and attribution (`where`, `summarize`, `count()`, `by`), smart filtering to separate signal from noise, and building visual dashboard reporting for stakeholders.
* **Sample Implementation:**
  ```kusto
  // Mapping Malicious Traffic by Country
  CommonSecurityLog
  | where DeviceAction != "denied" // Focusing on traffic that bypassed the perimeter
  | where MaliciousIP_Flag == true // Comparing against external threat intel lists
  | summarize ConnectionCount = count() by SourceIP, DestinationIP, SourceCountry
  | where ConnectionCount > 10
  | sort by ConnectionCount desc
  | render barchart with (title="Top Malicious Allowed Connections by Country")
  
### Azure Storage Account Logs & Diagnostics ✅
* **Investigative Impact:** Configured diagnostic settings to track both "Service" and "Blob" level metrics on Azure storage accounts used for sensitive data.
* **Key Takeaway:** Essential for spotting Account Takeover (ATO) or Data Exfiltration in real-time. *If you don't log it, you can't investigate it.*

---

## 📚 Hands-on Training & Labs

### 🐧 [Linux Fundamentals Part 1](https://tryhackme.com/room/linuxfundamentalspart1) *(TryHackMe)*
* **Outcome:** Mastered essential command-line interactions and terminal workflows.

### 🐍 [Python Basics](https://tryhackme.com/room/pythonbasics) *(TryHackMe)*
* **Outcome:** Learned code editor fundamentals and applied knowledge by building a short investment project.

### 🛡️ [SOC Fundamentals](https://app.letsdefend.io/training/lessons/soc-fundamentals) *(LetsDefend)*
* **Outcome:** Gained hands-on proficiency in core SOC workflows, SIEM log correlation, triage, distinguishing true/false positives, and mapping behaviors to the MITRE ATT&CK® framework.

### 🔓 [Offensive Security Intro](https://tryhackme.com/room/offensivesecurityintrokKx12) *(TryHackMe)*
* **Outcome:** Analyzed attacker methodologies across reconnaissance, enumeration, and exploitation phases using Nmap, GoBuster, and Metasploit to strengthen defensive postures and proactively identify security gaps.
---

## 📉 Growth & Metrics
* **Core Competencies Mastered:** Azure Storage Account Logs Setup, Azure Monitor Logs, and Advanced KQL Time-Series Analysis.
