# CV & Cover Letter Optimizer — a Claude Skill

A [Claude Skill](https://www.anthropic.com/news/skills) that turns a generic résumé/CV into a **targeted, interview-ready application package** for one of three tracks — a **job**, an **academic opportunity** (Master's / PhD / cotutelle / scholarship), or a **freelance/consulting gig** — and writes the matching cover letter. Final deliverables are **ATS-safe Word (`.docx`) files**.

Built with the `skill-creator` workflow. Author: **Juliana Quintana Rojas**. Licensed under MIT.

---

## What it does

The skill makes Claude act as a senior hiring manager / admissions chair / client lead in the target field, and runs a structured process instead of generic résumé tweaking.

**Step 0 — Establish the target.** You declare the track (job / academic / freelance) and provide the résumé, the target description (job posting, academic call, or RFP), and 1–2 peer organizations for tone calibration. For academic tracks it also requires your **actual research** (topic, methods, status, publications) and, for cotutelle, why the two institutions belong together.

**Part A — CV improvement (5 passes):**
1. **Brutal critique** — what's weak, missing, or reject-on-sight, from a real reviewer's perspective.
2. **ATS gap analysis** — missing keywords, under-highlighted skills, and bullet restructuring, compared against the actual posting/call.
3. **Bullet rewrite** — every bullet as *Action Verb + Task + Measurable Result*; the skill asks you for real numbers rather than inventing them.
4. **Voice calibration** — summary and skills rewritten to sound native to the target field.
5. **Final hardening** — tense consistency, cliché removal, and a strict **factual-standing rule**: the CV shows only your *current* reality and never presents the applied-for role/institution/status as if already held.

**Part B / C — The letter:**
- **Job / freelance:** a cover letter built on live company research (recent news, leadership, red flags), never opening with "I am writing to express my interest," connecting your experience to the role's top 3 needs, and ending with a specific call to action.
- **Academic:** a **Statement of Research** (the centerpiece) plus a **motivation letter**, with mandatory live research on the program and prospective advisors, and an explicit institutional-fit / cotutelle-bridge argument.

**Output:** ATS-safe `.docx` files (single-column, standard headings/fonts, no tables/text-boxes for content). See [`references/ats_rules.md`](cv-coverletter-optimizer/references/ats_rules.md).

---

## Repository contents

```
cv-coverletter-optimizer/
├── SKILL.md                  # the skill itself (instructions Claude follows)
└── references/
    ├── ats_rules.md          # ATS-safe formatting checklist
    └── examples.md           # before/after bullets, summaries, hooks (incl. academic)
cv-coverletter-optimizer.skill  # packaged, installable version
LICENSE                        # MIT
```

## How to use it

**Option A — install the packaged skill.** Download `cv-coverletter-optimizer.skill` and upload it in Claude where skills are managed (Settings → Capabilities/Skills). Then just upload your résumé and say e.g. *"Tailor my CV to this PhD call and write the motivation letter."*

**Option B — use the source directly.** Copy the `cv-coverletter-optimizer/` folder into your own skills setup (e.g. Claude Code's skills directory, or repackage it with the `skill-creator` packager).

> **Note:** This skill works best in a Claude environment that can create files (`.docx`) and search the web for the company/advisor research step.

## Requirements

- A Claude product that supports Skills and file creation.
- Web access for the live research step (Part B/C).

## Contributing

Issues and pull requests welcome — especially additional field-specific examples (more industries, more academic disciplines) in `references/examples.md`.

## License

MIT © 2026 Juliana Quintana Rojas. See [LICENSE](LICENSE).

## Acknowledgements

Scaffolded with Anthropic's `skill-creator`. Not affiliated with or endorsed by Anthropic.
# cv-coverletter-opt-claude
