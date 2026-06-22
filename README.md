# Azure Sentinel Threat Hunting Lab
## Project Overview

This project demonstrates the deployment of a cloud-based threat hunting environment using Microsoft Azure and Microsoft Sentinel. A Windows 11 virtual machine was onboarded through Azure Arc and Azure Monitor Agent (AMA) to collect endpoint telemetry and investigate simulated attacker reconnaissance activity.

The lab focused on collecting and analyzing PowerShell activity, command execution, and USB device telemetry while developing KQL queries, analytics rules, and dashboards for investigation and monitoring.
## Objectives
- Deploy Microsoft Sentinel and Log Analytics Workspace
- Onboard a Windows 11 VM through Azure Arc
- Configure Azure Monitor Agent (AMA)
- Enable PowerShell and event logging
- Simulate attacker reconnaissance techniques
- Investigate endpoint telemetry
- Develop KQL hunting queries
- Create analytics rules and dashboards
- Perform incident investigation and documentation
## Technologies Used
- Microsoft Azure
- Microsoft Sentinel
- Azure Arc
- Azure Monitor Agent (AMA)
- Log Analytics Workspace
- Windows 11 Virtual Machine
- PowerShell
- Kusto Query Language (KQL)
## Lab Workflow
1. Deployed Azure Resource Group and Log Analytics Workspace  
2. Enabled Microsoft Sentinel  
3. Onboarded Windows 11 VM using Azure Arc  
4. Installed Azure Monitor Agent (AMA)  
5. Enabled PowerShell and event logging  
6. Simulated attacker reconnaissance activity  
7. Collected endpoint telemetry in Sentinel  
8. Performed threat hunting using KQL  
9. Built analytics rules and dashboards  
10. Investigated USB and PowerShell activity
## Threat Simulation
The following reconnaissance commands were executed to simulate attacker behavior:
- whoami  
- hostname  
- ipconfig  
- Get-Process  
- Get-Service  
- Get-LocalUser  
- net user
## Investigation Summary
The investigation focused on:
- PowerShell execution activity
- Reconnaissance command usage
- USB device connection telemetry
- Endpoint event correlation using KQL
- Timeline analysis of suspicious activity
## Skills Demonstrated
- Threat Hunting
- SIEM Administration
- Endpoint Monitoring
- Windows Event Logging
- Log Analysis
- Incident Investigation
- Detection Engineering
- Security Monitoring
- Cloud Security Fundamentals
- KQL Query Development
## Screenshots
The `screenshots/` folder contains step-by-step evidence of:
- Azure environment setup
- Sentinel configuration
- Azure Arc onboarding
- AMA configuration
- PowerShell activity
- USB device detection
- Threat hunting queries
- Analytics rule creation
- Dashboard visualization
