---
name: Using VC Skills
description: Orientation + norms for the VC skills set; mirrors Superpowers' using-superpowers.
tags: [vc, meta]
---
# Using VC Skills

This plugin transforms rough thoughts, emails, and notes into polished, VC-ready content through **Socratic refinement + structured outputs**.

## Core Workflow

**Input**: Copy/paste thoughts, emails, investor Q&A, rough drafts
**Process**: Socratic questioning → poke holes → refine → structure
**Output**: Markdown files ready to copy/paste into decks, memos, data rooms

## Commands

**Primary workflows** (Socratic flows):
- `/vc:shoot-the-shit` — free‑flow dialog to explore angles (ideas > artifacts)
- `/vc:advice` — ask‑first advisory; options → trade‑offs → recommendation
- `/vc:research` — generates a **research plan** + **query set** (no execution)
- `/vc:stuck` — unblocker; 15‑minute micro‑plan with IF‑THENs
- `/vc:punch-it-up` — sharpen narratives and pitches with before/after rewrites

**Secondary skills** (available but not via `/vc:` commands):
- `fundraising-narrative-and-arc` — 10-12 slide story arc
- `tam-sam-som-triangulation` — Market sizing with 3 methods
- `problem-and-customer-pain` — Pain math and ICP definition
- `growth-motion-and-sales-design` — GTM motion and pipeline math
- `pricing-and-packaging` — Price ladders and packaging tiers
- `unit-economics-and-sensitivity` — LTV/CAC and sensitivity analysis
- `traction-metrics-and-milestones` — KPIs and milestone planning
- `competition-and-positioning` — Competitive matrix and positioning
- `defensibility-and-barriers` — Moat analysis and barriers to entry
- `pilots-and-case-studies` — Proof points and case study structure
- `use-of-funds-and-operating-plan` — Milestone-based use of funds
- `risk-matrix-and-mitigations` — Risk identification and mitigation plans
- `investment-readiness-audit` — Investor-readiness checklist
- `diligence-data-room-checklist` — Data room organization
- `regulatory-and-certification-deeptech` — Regulatory pathways for deeptech

## File Management Pattern

**MANDATORY**: All VC work uses this directory structure:

```
vc-work/
├── context.md              # Running accumulation of ALL inputs (thoughts, emails, Q&A)
├── session-logs/
│   └── YYYY-MM-DD-HH-MM.md # Log of each session (what was discussed, what was refined)
└── outputs/
    ├── investor-qa.md      # Structured Q&A for investors
    ├── narrative.md        # Fundraising narrative and arc
    ├── tam-analysis.md     # TAM/SAM/SOM analysis
    ├── gtm-plan.md         # Go-to-market plan
    └── [topic].md          # Other structured outputs
```

**At the start of EVERY session:**
1. Read `context.md` to load accumulated context
2. Create new session log: `session-logs/YYYY-MM-DD-HH-MM.md`

**During EVERY session:**
3. Append ALL new inputs to `context.md` (paste of thoughts/emails/notes)
4. Log all actions/decisions in current session log

**At the end of EVERY session:**
5. Write/update relevant `outputs/[topic].md` files
6. Ensure outputs are **copy/paste ready** (clean markdown, no meta-commentary)

## Defaults

- **Questions first**. Socratic refinement before writing.
- **Always create artifacts**. Every skill run produces a markdown file in `outputs/`.
- **Label assumptions**. If numbers matter, propose quick napkin math.
- **Define acronyms** when first used (e.g., **TAM/SAM/SOM**, **LTV/CAC**, **ICP**).
- **Cite sources**. Link to data, comps, or investor feedback.
- **Context accumulates**. Reference past sessions from `context.md`.

## When to Use Secondary Skills

Primary skills will **automatically reference** relevant secondary skills:
- `/vc:advice` preparing for investor meeting → load `fundraising-narrative`, `tam-sam-som`, `traction-metrics`
- `/vc:shoot-the-shit` about GTM → reference `growth-motion-and-sales-design`, `pricing-and-packaging`
- `/vc:punch-it-up` refining pitch → reference `problem-and-customer-pain`, `competition-and-positioning`

**Read the secondary SKILL.md** when you need its checklist/structure.

Use `/help` to see the commands after installation.
