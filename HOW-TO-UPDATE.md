# How to Keep This Repo Current

A portfolio that stops updating stops being useful. A simple routine to keep this one honest and current:

## Weekly (or after each study session)

1. Update the relevant `study-notes/0X-*.md` file — check off concepts studied, fill in the "In my own words" section for anything now understood.
2. Update `certifications/cysa-plus-progress-tracker.md` — objective statuses and the study log table.

## After every lab or hands-on exercise

1. Add a write-up to `practice-labs/` using the template in `practice-labs/README.md`.
2. Add a row to the log table in `practice-labs/README.md`.
3. Link it back from the relevant `study-notes/` file's "Practice tie-in" section.
4. Update proficiency levels in `tools/README.md` for any tool used.

## After building or finishing anything

1. Give it its own subfolder under `projects/` with a README (what it does, how to run it, what it demonstrates).
2. Add a row to `projects/README.md`.

## After investigating an incident (real or simulated)

1. Copy `incident-investigations/incident-report-template.md` into a dated file and fill it in.
2. If the investigation revealed a gap in the methodology, update `incident-investigations/investigation-methodology.md`.

## After any status change

The live site at [`docs/index.html`](./docs/index.html) is driven by a single `DATA` block near the bottom of that file — domains, objectives, tools, timeline, methodology, projects. Editing that one object updates the whole page; nothing else in the file needs touching.

So a status change usually lands in up to four places:

1. `study-notes/` — the domain file itself
2. `certifications/cysa-plus-progress-tracker.md` — the objective row
3. `docs/index.html` — the matching entry in `DATA`
4. `README.md` — the progress table, if a domain percentage moved

## Committing

Keep commits small and descriptive — each one should represent one study session, one lab, or one project update. This commit history is itself part of the portfolio: it shows consistency over time.

```bash
git add .
git commit -m "Add TryHackMe SOC Level 1 write-up + update Domain 1 notes"
git push
```
