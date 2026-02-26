# Len SOC Journey

## Overview
This repository documents my hands-on Security Operations Center (SOC) home lab. The goal is to simulate real-world attack scenarios, analyze system logs, develop detections, and practice structured incident response documentation.

This lab is built to strengthen practical SOC analyst skills through controlled attacker vs. victim simulations.

## Lab Architecture

**Victim Machine**
- Windows 11 (Pro)
- Sysmon telemetry
- Windows Event Logging
- PowerShell auditing enabled

**Attacker Machine**
- Kali Linux
- Network scanning and attack simulation tools

**Network Configuration**
- Bridged adapter configuration
- Same subnet attacker-to-victim simulation

## Objectives

- Improve attack pattern recognition
- Perform log-based investigations
- Develop detection logic
- Map activity to MITRE ATT&CK techniques
- Practice structured incident reporting

## Planned Attack Simulations

- Nmap scanning detection
- Brute force login attempts
- Encoded PowerShell execution
- Suspicious scheduled task persistence
- Malicious file download simulation
- Lateral movement testing (future phase)

## Repository Structure
home-lab/ → Lab architecture and setup documentation
incident-reports/ → Structured investigation writeups
detections/ → Detection logic and rule development
notes/ → Research and reference materials

## Current Phase

Building Windows 11 victim baseline and enabling advanced telemetry.
