# Lab Walkthrough

## Environment Setup
A cloud-based monitoring environment was built using Microsoft Azure and Microsoft Sentinel to simulate endpoint threat detection and investigation.

- Created Azure Resource Group (CyberLab-RG)
- Deployed Log Analytics Workspace (CyberLAW)
- Enabled Microsoft Sentinel for SIEM capabilities
- Onboarded Windows 11 VM using Azure Arc
- Installed Azure Monitor Agent (AMA) for log collection
- Enabled PowerShell and Windows event logging for endpoint visibility

---

## Threat Simulation
To simulate attacker reconnaissance behavior, the following commands were executed on the Windows VM:

- whoami
- hostname
- ipconfig
- Get-Process
- Get-Service
- Get-LocalUser
- Get-ChildItem C:\Users
- net user

A USB device was also connected to generate endpoint-level event telemetry.

---

## Investigation Process
Threat hunting was performed using Microsoft Sentinel and KQL queries.

The investigation focused on:

- PowerShell execution activity
- Reconnaissance command usage
- Endpoint telemetry analysis
- USB device event detection (Event ID 400/410)
- Timeline correlation of system activity
- Incident validation using Sentinel analytics rules
- Visualization of activity using dashboards

---

## Screenshot Evidence Walkthrough

01 – Windows VM Desktop  
Initial baseline environment of Windows 11 virtual machine.

02 – Azure Portal  
Azure resource configuration and management interface.

03 – Resource Group  
Creation of CyberLab-RG used to contain all lab resources.

04 – Log Analytics Workspace  
Workspace configured for centralized log ingestion.

05 – Microsoft Sentinel Overview  
SIEM environment enabled for threat detection and hunting.

06 – Azure Arc Script  
Onboarding script generated for VM connection.

07 – Azure Arc Connected  
Successful connection of Windows VM to Azure Arc.

08 – Azure Arc Machine  
Verification of endpoint registration in Azure.

09 – AMA Connector  
Azure Monitor Agent configured for log collection.

10 – Logging Configuration  
PowerShell and Windows event logging enabled for telemetry visibility.

11 – Suspicious PowerShell Activity  
Execution of reconnaissance commands for threat simulation.

12 – USB Device Connected  
USB insertion generating Event ID 400/410 telemetry.

13 – PowerShell Events  
Detected PowerShell execution logs within Sentinel.

14 – Recon Hunting  
KQL queries used to identify suspicious activity.

15 – USB PowerShell Investigation  
Correlation between USB and endpoint activity.

16 – Analytics Rule  
Scheduled detection rule created for PowerShell activity.

17 – Recon Activity Dashboard and Timeline  
Visualization of endpoint activity over time.

18 – Most Executed Recon Commands  
Analysis of command frequency during simulation.

19 – Recon Investigation Details  
Final investigation summary and validation of findings.
