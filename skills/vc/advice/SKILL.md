---
name: Advice (Socratic)
description: Ask‑first advisory flow; we question before recommending.
tags: [vc, socratic]
---
# Advice (Socratic)

Deliver pointed advice only *after* a brief clarifying interview.

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user to paste their question/situation → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
4. **Auto-load secondary skills** (see section below)

## Auto-Load Secondary Skills (MANDATORY)

After receiving the user's question/situation, scan for keywords and **use the Skill tool** to load relevant secondary skills **before** beginning the Socratic flow.

**Keyword triggers → Skills to load**:
- "fundraise", "investor", "deck", "pitch", "raise" → `skills/secondary/fundraising-narrative-and-arc`
- "market", "TAM", "SAM", "SOM", "market size" → `skills/secondary/tam-sam-som-triangulation`
- "traction", "metrics", "KPIs", "milestones", "growth" → `skills/secondary/traction-metrics-and-milestones`
- "GTM", "go-to-market", "sales", "pipeline", "funnel" → `skills/secondary/growth-motion-and-sales-design`
- "pricing", "packaging", "price", "tiers", "discount" → `skills/secondary/pricing-and-packaging`
- "unit economics", "CAC", "LTV", "gross margin", "payback" → `skills/secondary/unit-economics-and-sensitivity`
- "ICP", "customer", "pain", "buyer", "problem" → `skills/secondary/problem-and-customer-pain`
- "competitors", "competitive", "positioning" → `skills/secondary/competition-and-positioning`
- "moat", "defensibility", "barriers" → `skills/secondary/defensibility-and-barriers`
- "ready", "readiness", "audit", "checklist" → `skills/secondary/investment-readiness-audit`

**Instructions**:
1. Use the **Skill tool** to load each matched skill
2. Read and absorb the Core Questions and Artifacts from each loaded skill
3. Synthesize questions across all loaded skills + the Advice flow
4. Proceed with Turn structure below

## Turn structure
1) **Frame** — restate the crux; "what outcome are you optimizing for?"
2) **Probe** — ≤5 Qs: constraints, time horizon, risk tolerance, resources, success KPI. **Include questions from loaded secondary skills.**
3) **Options** — 2–3 viable paths w/ trade‑offs (speed, cost, risk, learning).
4) **Recommendation** — pick one path and say why; first 3 moves.
5) **Commit** — decision or data request to break the tie.

## Micro‑commands
- `push` — tighten recommendation (shorter timeline, higher intensity)
- `widen` — add a contrarian or non‑obvious option
- `evidence` — list the data that would flip the recommendation

## MANDATORY Output

**Always create/update**: `vc-work/outputs/advice-[topic].md`

**Format**:
```markdown
# Advice: [Topic]
**Date**: YYYY-MM-DD
**Context**: [1-2 sentence framing of the question]

## Question
[Original question/situation from user]

## Clarifying Probe
[Answers to the 5 probing questions]

## Options
### Option 1: [Name]
- **Trade-offs**: Speed ☐ | Cost ☐ | Risk ☐ | Learning ☐
- **Description**: [What this path looks like]

### Option 2: [Name]
- **Trade-offs**: Speed ☐ | Cost ☐ | Risk ☐ | Learning ☐
- **Description**: [What this path looks like]

### Option 3: [Name] (if applicable)
- **Trade-offs**: Speed ☐ | Cost ☐ | Risk ☐ | Learning ☐
- **Description**: [What this path looks like]

## Recommendation
**Pick**: [Option X]
**Why**: [Rationale in 2-3 sentences]

### First 3 Moves
1. [Action 1 with timeline]
2. [Action 2 with timeline]
3. [Action 3 with timeline]

## Decision / Next Data Needed
[What decision needs to be made, or what data would change the recommendation]

## Related Skills
[List any secondary skills that should be loaded next, e.g., "Load `tam-sam-som-triangulation` to validate market size assumptions"]
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
