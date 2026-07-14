# 🛡️ Home SOC Lab - Splunk Cloud & Sysmon

![Status](https://img.shields.io/badge/Status-In%20Progress-green)
![Platform](https://img.shields.io/badge/Platform-Windows%2011-blue)
![SIEM](https://img.shields.io/badge/SIEM-Splunk%20Cloud-orange)

## Overview

This project documents the development of a Security Operations Center (SOC) home lab designed to emulate enterprise endpoint monitoring and detection workflows.

The lab currently collects Windows Event Logs and Sysmon telemetry from a Windows 11 endpoint using the Splunk Universal Forwarder and forwards the data to Splunk Cloud for centralized log analysis, threat hunting, and detection engineering.

The long-term goal is to expand this environment into a multi-host detection lab capable of simulating attacker behavior, building SPL detections, and documenting investigations aligned with the MITRE ATT&CK framework.

---

## Objectives

- Deploy Splunk Cloud as a SIEM
- Collect Windows Event Logs
- Deploy Sysmon for endpoint telemetry
- Develop SPL detection queries
- Map detections to MITRE ATT&CK
- Simulate attacker techniques
- Build dashboards for security monitoring
- Document detection engineering workflows

---

# Current Architecture

(Add architecture diagram here)

---

## Current Environment

| Component | Status |
|------------|--------|
| Windows 11 Endpoint | ✅ |
| Splunk Cloud | ✅ |
| Splunk Universal Forwarder | ✅ |
| Windows Event Logs | ✅ |
| Sysmon | ✅ |
| Dashboards | 🚧 |
| MITRE ATT&CK Detections | 🚧 |
| Atomic Red Team | ⏳ |
| Active Directory | ⏳ |

---

# Data Sources

Currently ingesting:

### Windows Event Logs

- Security
- System
- Application

### Sysmon

- Event ID 1 – Process Creation
- Event ID 3 – Network Connections
- Event ID 11 – File Creation
- Event ID 13 – Registry Modifications
- Event ID 22 – DNS Queries

---

# Current Detections

| Detection | Status |
|------------|--------|
| Process Creation | ✅ |
| PowerShell Execution | 🚧 |
| Failed Logon Detection | 🚧 |
| Registry Modification | 🚧 |
| DNS Monitoring | 🚧 |

---

# Repository Structure

```text
architecture/
detections/
spl/
dashboards/
screenshots/
docs/
attack-simulations/
```

---

# Example SPL Searches

Example searches are stored under

```
spl/
```

Examples include:

- Process Creation
- PowerShell Execution
- Failed Logons
- Registry Changes
- DNS Queries

---

# MITRE ATT&CK Coverage

| Technique | Detection |
|------------|-----------|
| T1059.001 | PowerShell |
| T1112 | Registry Modification |
| T1071.004 | DNS |
| T1078 | Valid Accounts (planned) |

---

# Screenshots

## Windows Event Logs

(Add Screenshot)

## Sysmon Process Creation

(Add Screenshot)

## Splunk Search Results

(Add Screenshot)

## Dashboard

(Add Screenshot)

---

# Roadmap

## Phase 1 ✅

- Install Splunk Universal Forwarder
- Connect to Splunk Cloud
- Install Sysmon
- Verify telemetry ingestion

## Phase 2 🚧

- Failed Logon Detection
- PowerShell Detection
- Registry Monitoring
- Dashboard Development

## Phase 3

- Atomic Red Team
- MITRE ATT&CK Detection Library
- Detection Validation
- Incident Reports

## Phase 4

- Active Directory
- Multi-endpoint Monitoring
- Attack Simulation
- Threat Hunting

---

# Skills Demonstrated

- Windows Administration
- SIEM Deployment
- Splunk SPL
- Windows Event Logging
- Sysmon
- Detection Engineering
- Threat Hunting
- Log Analysis
- MITRE ATT&CK

---

# References

- Splunk Documentation
- Sysinternals Sysmon
- MITRE ATT&CK
