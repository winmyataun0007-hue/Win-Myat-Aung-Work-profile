# Domain 1.0 — Security Operations (33% of exam)

**Status:** 🟡 In progress
**Last updated:** _fill in when you edit this file_

## Objectives covered

- 1.1 — Explain the importance of system and network architecture concepts in security operations
- 1.2 — Given a scenario, analyze indicators of potentially malicious activity
- 1.3 — Given a scenario, use appropriate tools or techniques to determine malicious activity
- 1.4 — Compare and contrast threat-intelligence and threat-hunting concepts
- 1.5 — Explain the importance of efficiency and process improvement in security operations

## Key concepts

### 1.1 System and network architecture

- [ ] Logging levels and log sources (OS, application, network device, cloud)
- [ ] Log ingestion — pull vs. push, agent-based vs. agentless
- [ ] Operating system concepts relevant to SOC work (Windows Event Log, Linux syslog/auditd)
- [ ] Infrastructure concepts: on-prem vs. cloud vs. hybrid, virtualization, containerization
- [ ] Network architecture: network segmentation, zero trust, SASE, IaC
- [ ] Identity and access management concepts (federation, MFA, PAM, SSO)
- [ ] Encryption and sensitive data protection basics as they relate to detection

### 1.2 Analyzing indicators of malicious activity

- [ ] Network-related indicators (traffic spikes, beaconing, rogue devices, scans)
- [ ] Host-related indicators (unauthorized processes, unauthorized scheduled tasks, registry changes)
- [ ] Application-related indicators (anomalous activity, unexpected outbound connections, error messages)
- [ ] Other indicators: social engineering attempts, obfuscated/encoded payloads

### 1.3 Tools and techniques for determining malicious activity

- [ ] Packet capture (Wireshark, tcpdump)
- [ ] SIEM correlation searches
- [ ] Endpoint detection and response (EDR) telemetry
- [ ] Log analysis and log aggregation platforms
- [ ] Scripting for parsing/automation (Python, PowerShell, Bash basics)

### 1.4 Threat intelligence vs. threat hunting

- [ ] Threat intelligence lifecycle (requirements → collection → processing → analysis → dissemination → feedback)
- [ ] Intelligence sources: OSINT, closed-source, ISACs, commercial feeds
- [ ] Indicators of compromise (IOCs) vs. tactics, techniques, and procedures (TTPs)
- [ ] MITRE ATT&CK framework — how it's structured and used
- [ ] Threat hunting methodology: hypothesis-driven vs. IOC-driven vs. TTP-driven
- [ ] Difference between reactive (alert-driven) and proactive (hunting) detection

### 1.5 Efficiency and process improvement

- [ ] SOAR (Security Orchestration, Automation, and Response) concepts
- [ ] Playbooks and runbooks
- [ ] Alert tuning and reducing false positives
- [ ] Technology and workflow integration to reduce analyst fatigue

## In my own words

_Write a short explanation of each sub-objective above in plain language, without looking at notes. If you can't do it yet, that's the signal to keep studying — leave this section honest rather than filling it with copied definitions._

## Practice tie-in

_Links to entries in [`../practice-labs/`](../practice-labs) that exercised this domain will go here once completed._

## Resources used

- _List courses, books, videos, and practice platforms as you use them._
