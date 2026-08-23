# Practice Labs

Write-ups of hands-on exercises. Every entry here reflects something I actually did, not something I read about — that's the line between this folder and `study-notes/`.

## Log format

Add one row per completed lab and link to its write-up file (`YYYY-MM-DD-short-title.md`):

| Date | Platform | Scenario | Domain(s) exercised | Write-up |
|---|---|---|---|---|
| _example_ | _e.g. TryHackMe_ | _e.g. "SOC Level 1 — Log Analysis room"_ | Security Operations | _link_ |

## Recommended platforms for CySA+-aligned practice

- **TryHackMe** — SOC Level 1 & 2 learning paths, log analysis, SIEM rooms
- **LetsDefend** — SOC analyst simulation, real alert triage
- **Blue Team Labs Online** — investigation challenges, digital forensics
- **CyberDefenders** — blue team CTF-style incident investigations
- **Splunk BOTS (Boss of the SOC)** — free public dataset for SIEM practice
- **Home lab** — Security Onion or ELK stack ingesting simulated attack traffic

## Write-up template

Use this structure for each lab write-up:

```markdown
# [Lab/Room Name] — [Platform]

**Date completed:**
**Domain(s) exercised:** (Security Operations / Vulnerability Management / Incident Response / Reporting)
**Tools used:**

## Scenario
What was the setup/premise?

## Approach
What did I actually do, step by step?

## Findings
What did I find? (IOCs, root cause, misconfig, etc.)

## What I learned
What's new to me, or what clicked that hadn't before?

## What I'd do differently
Honest reflection — faster path, missed indicator, better tool choice.
```

Nothing gets added to the log table above until a full write-up exists.
