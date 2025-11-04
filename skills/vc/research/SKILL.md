---
name: Research Plan (Socratic)
description: Generates a research plan and query set for external tools; no execution.
tags: [vc, socratic]
---
# Research Plan (Socratic)

**This does not do research.** It interrogates the brief and emits a plan + query set usable by tools (e.g., DeepResearch).

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for research objective → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
4. **Auto-load secondary skills** (see section below)

## Auto-Load Secondary Skills (MANDATORY)

After receiving the user's research objective, scan for keywords and **use the Skill tool** to load relevant secondary skills **before** beginning the research planning.

**Keyword triggers → Skills to load**:
- "market", "TAM", "SAM", "SOM", "market size" → `skills/secondary/tam-sam-som-triangulation`
- "competitors", "competitive", "positioning", "landscape" → `skills/secondary/competition-and-positioning`
- "regulatory", "compliance", "certification", "standards" → `skills/secondary/regulatory-and-certification-deeptech`
- "diligence", "data room", "DD", "due diligence" → `skills/secondary/diligence-data-room-checklist`
- "moat", "defensibility", "barriers" → `skills/secondary/defensibility-and-barriers`
- "ICP", "customer", "pain", "buyer", "problem" → `skills/secondary/problem-and-customer-pain`
- "GTM", "go-to-market", "sales", "pipeline" → `skills/secondary/growth-motion-and-sales-design`
- "traction", "metrics", "KPIs", "milestones" → `skills/secondary/traction-metrics-and-milestones`

**Instructions**:
1. Use the **Skill tool** to load each matched skill
2. Read and absorb the Core Questions and Artifacts from each loaded skill
3. Synthesize research questions across all loaded skills + the Research Plan flow
4. Proceed with Turn structure below

## Turn structure
1) **Scope** — objective, audience, decision, deadline. **Include context from loaded secondary skills.**
2) **Horizon** — recency window, geos, industries, exclusions.
3) **Sources** — primary vs secondary; target orgs/datasets/filings.
4) **Queries** — operators, synonyms, entity variants. **Include queries informed by loaded secondary skills.**
5) **Plan** — phased checklist with stop conditions and deliverables.

## Secondary skills to reference (when relevant)
- `tam-sam-som-triangulation` — if researching market size
- `competition-and-positioning` — if researching competitive landscape
- `regulatory-and-certification-deeptech` — if researching regulatory/compliance
- `diligence-data-room-checklist` — if preparing for diligence

## Micro‑commands
- `tighten` — narrow scope/recency; fewer sources, higher quality
- `spray` — expand scope; more adjacencies, long‑tail terms
- `cite-style:<apa|chicago|linklist>` — set citation style

## MANDATORY Output

**Always create/update**: `vc-work/outputs/research-plan-[topic].md`

**Format** (YAML + Markdown):
```markdown
# Research Plan: [Topic]
**Date**: YYYY-MM-DD

## Research Brief
**Objective**: [One sentence]
**Decision this will inform**: [What decision/outcome]
**Deadline**: [ISO date]

## Research Plan (YAML)

\`\`\`yaml
objective: <one sentence>
decision: <what this will inform>
deadline: <ISO date>
recency: <e.g., 90d>
scope:
  geos: [ ]
  industries: [ ]
  exclusions: [ ]
sources:
  primary: [interviews, surveys]
  secondary: [10-K, 8-K, standards bodies, trade press]
queries:
  seed: [ ]
  operators: ["site:", "filetype:", "intitle:", "after:"]
  entities: [ ]
deliverables:
  - memo_outline
  - table_of_sources
stops:
  - budget_exhausted
  - n>=3 independent confirmations for key claims
\`\`\`

## Search Queries (Copy/Paste Ready)
1. [Query 1]
2. [Query 2]
3. [Query 3]

## Phased Execution Plan
### Phase 1: [Name] (Days 1-X)
- [ ] [Task 1]
- [ ] [Task 2]

### Phase 2: [Name] (Days X-Y)
- [ ] [Task 1]
- [ ] [Task 2]

## Deliverables Checklist
- [ ] Memo outline
- [ ] Table of sources with citations
- [ ] [Other deliverables]

## Stop Conditions
- Budget exhausted ($ or hours)
- n>=3 independent confirmations for key claims
- [Other stop conditions]
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
