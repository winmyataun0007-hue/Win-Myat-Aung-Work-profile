# Zane — SOC Analyst Portfolio & CySA+ Study Log

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/win-myat-aung-46630a35b/)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Profile-212C42?style=flat-square&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/winmyataun0007)

Cybersecurity portfolio and public study log documenting my path into a Security Operations Center (SOC) analyst role. This repository is a working record — it grows as I study, practice, and build.

**Target roles:** SOC Analyst (Tier 1/2) · Blue Team · Security Operations · Security Monitoring · Junior Incident Response · IT Help Desk (security-track)
**Current certification goal:** CompTIA CySA+ (CS0-003)

---

## About this repository

Most portfolios only show finished work. This one is deliberately different — it also shows the *process*: what I'm studying right now, what I actually understand versus what I'm still working through, and how my hands-on practice maps back to real SOC responsibilities. Recruiters and hiring managers can watch this repo mature over time.

| | |
|---|---|
| **Status** | 🟡 Actively studying for CompTIA CySA+ (CS0-003) |
| **Study started** | August 2026 |
| **Last updated** | See commit history |

---

## Repository map

| Folder | What's in it |
|---|---|
| [`study-notes/`](./study-notes) | Notes organized by CySA+ exam domain — what I've studied and what I understand |
| [`practice-labs/`](./practice-labs) | Write-ups from hands-on labs and ranges (TryHackMe, LetsDefend, Blue Team Labs Online, CyberDefenders, home lab) |
| [`projects/`](./projects) | Things I've built — detection rules, scripts, dashboards, small tools |
| [`tools/`](./tools) | Cheat sheets for the tools I can use, organized by SOC function |
| [`incident-investigations/`](./incident-investigations) | My investigation methodology and a reusable incident report template |
| [`certifications/`](./certifications) | CySA+ exam-objective progress tracker |

---

## 1. What I have studied

See [`study-notes/`](./study-notes) for full notes, organized by the four CompTIA CySA+ (CS0-003) exam domains:

- [Security Operations](./study-notes/01-security-operations.md) — 33% of exam
- [Vulnerability Management](./study-notes/02-vulnerability-management.md) — 30% of exam
- [Incident Response & Management](./study-notes/03-incident-response-management.md) — 20% of exam
- [Reporting & Communication](./study-notes/04-reporting-communication.md) — 17% of exam

Live progress against every exam objective: [`certifications/cysa-plus-progress-tracker.md`](./certifications/cysa-plus-progress-tracker.md).

## 2. What I understand

Each study-notes file ends with a plain-language "in my own words" section — a self-check that I can explain the concept without notes, not just recognize it on a multiple-choice question. This is how I catch the difference between *recognizing* a term and *understanding* it.

## 3. What I have practiced

Logged in [`practice-labs/`](./practice-labs) as I complete them — platform, scenario, tools used, and what I learned. Nothing is listed until it's actually done.

## 4. What I have built

Logged in [`projects/`](./projects) as I ship them. Planned early projects:

- A home SOC lab (Security Onion / ELK or Splunk Free, with simulated attack traffic)
- Detection rules/queries written against real log samples
- A small script that automates a repetitive analyst task (e.g., IOC lookups, log parsing)

## 5. What tools I can use

Tracked in [`tools/`](./tools), grouped by function (SIEM, packet analysis, EDR/host forensics, vulnerability scanning, threat intel, scripting). Each entry is marked with an honest proficiency level — exposure vs. working knowledge vs. comfortable using unsupervised.

## 6. How I investigate security incidents

My working investigation methodology (detection → triage → analysis → containment → eradication → recovery → lessons learned) is documented in [`incident-investigations/investigation-methodology.md`](./incident-investigations/investigation-methodology.md), aligned to the CySA+ incident response domain and NIST SP 800-61.

## 7. How I document technical findings

Every investigation I run gets written up using the reusable template in [`incident-investigations/incident-report-template.md`](./incident-investigations/incident-report-template.md), so findings are consistent, reproducible, and readable by both technical and non-technical stakeholders.

---

## Why this repo exists

I'm building toward a junior SOC analyst / blue team role. This repository is proof of consistent, honest effort — not a highlight reel. Entries are only added once the work is actually done, and unfinished sections say so rather than being padded out.

## Connect

- **LinkedIn:** [linkedin.com/in/win-myat-aung-46630a35b](https://www.linkedin.com/in/win-myat-aung-46630a35b/)
- **TryHackMe:** [tryhackme.com/p/winmyataun0007](https://tryhackme.com/p/winmyataun0007) — live record of rooms completed, badges, and learning paths in progress; the curated write-ups in [`practice-labs/`](./practice-labs) pull from this activity

Feel free to open an issue or reach out if you'd like to discuss any of the write-ups here.
