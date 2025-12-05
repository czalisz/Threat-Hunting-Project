# Threat-Hunting-Project
#Summary Overview
This project is a practical, hands-on SOC Threat Hunting lab designed to demonstrate my ability to identify and investigate malicious activity using Splunk and Sysmon. Using a Windows 11 Pro virtual machine, I recreated real-world attacker behaviors and analyzed the resulting telemetry to detect suspicious processes, persistence mechanisms, and network anomalies.

The goal of this project is to showcase how I approach threat hunting the way modern SOC analysts do—by forming hypotheses, running targeted Splunk queries, validating activity against MITRE ATT&CK techniques, and documenting clear findings. In addition to host-based detections, I included several foundational network investigation queries that reflect the types of threats businesses encounter daily.

This repository highlights my ability to work with logs, build detections, interpret security events, and communicate findings in a clear and structured way. 

## Objective
- Learn event log analysis
- Build Splunk hunting queries
- Detect attacker tradecraft
- Map findings to MITRE ATT&CK

## Tools Used
- Splunk Enterprise
- Splunk Universal Forwarder
- Sysmon
- MITRE ATT&CK
- Windows 11 Pro VM

## Key Findings
Successful detection of obfuscated PowerShell
Process injection using rundll32
Registry persistence creation
DNS query enumeration
Network recon

#Limitations
While this project demonstrates practical threat hunting skills using Splunk and Sysmon, the lab environment has several inherent limitations that differ from a real-world enterprise SOC:
Single-Host Environment - This lab uses a single Windows 11 VM as both the victim host and event-forwarding source. Because of this, the following limitations apply:
- No lateral movement visibility
- no multi-host pattern correlation
- no domain-based events

Limited Log Sources - The detections are based primarily on:
- Sysmon process creation, registry, network events
- Windows Event Logs
Log sources that you would in real SOC environments find that I could not include:
- EDR alerts
- Firewall logs
- DNS Server logs
- Email security tools
- Authentication logs
- Cloud logs

Non-Advanced Attack Simulation - The attacks recreated in this lab intentionally use:
- Simple command-line executions
- Basic LOLBins
- Straightforward persistence techniques
- No obfuscation beyond basic PowerShell encoding
Real-world adversaries often use:
- Multi-stage payloads
- Sophisticated obfuscation
- Signed malware
- Living-off-the-land with evasion layers
- Privilege escalation
- Credential dumping
- Lateral movement techniques

No Alerting or Automation Layer - This project focuses on manual hunting, not:
- Creating automated Splunk alerts
- Using SOAR playbooks
- Escalation workflows
- Ticketing System Integration
