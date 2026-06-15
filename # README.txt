# Project 2: IP Analysis with VirusTotal

## 📌 Overview
This project focuses on analyzing captured network traffic, extracting IP addresses, and validating them against the VirusTotal threat intelligence platform. The goal is to identify potentially malicious indicators and document the findings in a structured way.

## 🎯 Objectives
- Capture and inspect network traffic using Wireshark/tcpdump.
- Extract IP addresses from the traffic.
- Query VirusTotal API for verdicts on each IP.
- Document results with screenshots.
- Map findings to MITRE ATT&CK techniques.

## 🛠 Tools & Environment
- **Wireshark / tcpdump** → Packet capture
- **Python 3.11** → Scripting
- **Requests library** → API calls
- **VirusTotal API** → Threat intelligence
- **Google Drive** → Evidence storage (screenshots)
- **GitHub** → Code and documentation repository

## 🔍 Workflow
1. Captured traffic and extracted IPs.
2. Queried VirusTotal for each IP.
3. Collected verdicts (harmless, malicious, suspicious, undetected).
4. Stored evidence (screenshots in Google Drive).
5. Prepared documentation and GitHub repo.

## 📊 Results
- **172.24.201.165** → Harmless (70 engines flagged safe).
- **172.24.201.35** → Harmless (68 engines flagged safe).
- **192.46.211.253** → Malicious (2 engines flagged, 1 suspicious).
- **148.113.49.96** → No data found (private IP).

Screenshots of VirusTotal verdicts are available in the linked Google Drive folder.

## 🧩 MITRE ATT&CK Mapping
- **Malicious IP flagged** → T1071.001 (Command and Control: Web Traffic)  
- **Suspicious DNS/IP behavior** → T1071.004 (Command and Control: DNS)  
- **Potential flood traffic (if observed)** → T1499 (Impact: Endpoint Denial of Service)  

This mapping connects the observed indicators to adversary tactics, showing how attackers might leverage IPs for command‑and‑control or denial‑of‑service activities.

## 📂 Evidence
- Screenshots: [view screenshots here!][https://drive.google.com/drive/folders/11ixHsB9-x3KA-rhlCpL4kjE8rbYQg_WS]
- Script: `vt_check.py`  

## 👩‍💻 Author
Malinee — Cybersecurity Intern