# Projects — Things I've Built

Unlike `practice-labs/` (guided exercises on other platforms), this folder is for things I built myself, end to end.

## Log format

| Project | Description | Stack/Tools | Status | Link |
|---|---|---|---|---|
| **TriageDesk** | SOC alert triage & incident management platform: ingests Wazuh/Suricata alerts, enriches, risk-scores and correlates them into incidents, tracks SLAs (MTTA/MTTR) and maps to MITRE ATT&CK with playbooks. University capstone. | Python, FastAPI, SQLite, pytest | ✅ Shipped | [Repo](https://github.com/winmyataun0007-hue/Triagedesk) · [Live demo](https://winmyataun0007-hue.github.io/Triagedesk/demo/) |

## Planned projects

These are on the roadmap — moved into the table above (with their own subfolder) once there's real, working output:

- [ ] **Home SOC lab** — Security Onion or ELK stack ingesting logs, with simulated attack traffic (e.g. Atomic Red Team) to practice detection end-to-end
- [ ] **Detection rule pack** — a small set of Sigma or Splunk/ELK detection rules written against real or sample log data, with notes on why each rule was written the way it was
- [ ] **IOC lookup automation** — a Python script that takes a list of indicators (IPs/hashes/domains) and checks them against threat intel sources (e.g. VirusTotal, AbuseIPDB APIs)
- [ ] **Log parsing utility** — a script that normalizes/parses a messy log format into something a SIEM can ingest cleanly
- [ ] **Phishing analysis workflow** — a documented, repeatable process (plus supporting scripts) for triaging a suspicious email end to end

Each project, once started, gets its own subfolder here with its own README (what it does, how to run it, what it demonstrates) rather than living only in this index.
