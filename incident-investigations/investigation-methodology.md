# Incident Investigation Methodology

My working process for investigating a security incident, from initial alert to closure. Based on the NIST SP 800-61 (Computer Security Incident Handling Guide) lifecycle and the CySA+ CS0-003 Incident Response & Management domain (3.0).

This is a living document — it gets refined every time I run through a real investigation or lab and learn something the process didn't account for.

## The lifecycle

```
Preparation → Detection & Analysis → Containment → Eradication → Recovery → Post-Incident Activity
      ^______________________________________________________________________________|
                              (lessons learned feed back into preparation)
```

### 1. Preparation

Done *before* an incident happens.

- Know the environment: asset inventory, network diagram, normal baseline behavior
- Have access to the right tools before you need them (SIEM, EDR, packet capture)
- Know the escalation path and who needs to be told what
- Have a report template ready (see [`incident-report-template.md`](./incident-report-template.md)) so documentation starts on time one, not as an afterthought

### 2. Detection & Analysis

- **Triage the alert.** What fired it? Is it a known false positive pattern? What's the initial severity?
- **Gather context.** Pull related logs — not just the triggering event, but what happened before and after, on the same host/user/IP.
- **Validate.** Is this actually malicious, or a benign explanation (scheduled task, approved change, known tool)?
- **Scope.** What else is affected? Same technique used elsewhere? Same account, same subnet, same time window?
- **Map to a framework.** Where does this fit on MITRE ATT&CK / the Cyber Kill Chain? This drives what to look for next.
- **Determine severity and priority** based on scope, asset criticality, and business impact.

### 3. Containment

- **Short-term containment** — stop the bleeding without destroying evidence (isolate host, disable account, block IOC at the firewall/proxy)
- **Evidence preservation** — before doing anything destructive, capture what's needed (memory image, disk image, relevant logs) if forensics may be required
- **Long-term containment** — apply a more durable fix while planning eradication (e.g., temporary segmentation, patch staged for deployment)

### 4. Eradication

- Remove the actual root cause, not just the symptom (e.g., don't just delete the malware — find and close the entry vector)
- Patch the exploited vulnerability
- Reset compromised credentials
- Verify no persistence mechanisms remain (scheduled tasks, registry run keys, rogue accounts, web shells)

### 5. Recovery

- Restore systems from known-good backups or rebuild if trust in the system can't be re-established
- Monitor closely post-recovery for signs of reinfection or attacker return
- Confirm with stakeholders before returning systems to production

### 6. Post-Incident Activity

- **Lessons-learned review** — what worked, what didn't, what would speed up detection next time
- **Root cause analysis** — documented, not just discussed
- **Update detection rules/playbooks** based on what was learned
- **Final report** — written using [`incident-report-template.md`](./incident-report-template.md) and shared with the appropriate audience (see Domain 4.0 notes: [`../study-notes/04-reporting-communication.md`](../study-notes/04-reporting-communication.md))
- **Metrics** — capture time-to-detect and time-to-respond for this incident to track improvement over time

## Principles I try to hold to

- **Document as you go**, not after the fact — memory of exact timestamps and commands fades fast
- **Don't assume malicious or assume benign** — validate with evidence before either
- **Preserve evidence before you act**, when there's any chance forensics will matter
- **Communicate proportionally** — don't escalate everything to "critical," don't sit on something that actually is
