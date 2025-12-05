# Threat-Hunting-Project
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
