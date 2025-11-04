---
name: TAM/SAM/SOM Triangulation
description: Triangulate market size using 3 methods: bottoms‑up, tops‑down, and analog comps.
when_to_use: Any time a market number appears in a deck or memo.
version: 1.0.0
languages: all
---
# TAM/SAM/SOM Triangulation

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for market sizing data/assumptions → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- Bottoms‑up: # of buyers × ACV (annual contract value) or device count × ASP.
- Tops‑down: Credible third‑party spend pools; filter to SAM by constraints.
- Comps: Analog products/roll‑outs (price × penetration × time).

## Quick Reference
- State **assumptions** explicitly; show min/base/max; cite sources.
- Separate **device sales** vs **service/recurring**.
- Tie SOM to your next 24 months of capacity + channels.

## Artifacts
- 1 table: methods × outputs × sources; sensitivity band.

## Common Mistakes
- Quoting TAM without path to SAM/SOM.
- Ignoring channel and capacity constraints.

## MANDATORY Output

**Always create/update**: `vc-work/outputs/tam-sam-som-[market].md`

**Format**:
```markdown
# TAM/SAM/SOM Analysis: [Market Name]
**Date**: YYYY-MM-DD

## Input Data / Assumptions
[Paste of user's market sizing data from context.md]

## Three-Method Triangulation

### Method 1: Bottoms-Up
**Formula**: # of buyers × ACV (or device count × ASP)

**Calculation**:
- **# of buyers**: [number] ([source])
- **ACV** (or ASP): $[amount] ([source])
- **TAM (Bottoms-up)**: $[X]M

**Assumptions**:
- [Assumption 1]
- [Assumption 2]

### Method 2: Tops-Down
**Formula**: Credible third-party spend pool → filter to SAM by constraints

**Calculation**:
- **Total addressable spend**: $[X]M ([source: Gartner, IDC, etc.])
- **Constraints applied**:
  - [Constraint 1]: reduces to $[Y]M
  - [Constraint 2]: reduces to $[Z]M
- **SAM (Tops-down)**: $[Z]M

**Sources**:
- [Source 1]
- [Source 2]

### Method 3: Analogcomps
**Formula**: Analog product × penetration × time

**Calculation**:
- **Analog product/market**: [Name] achieved $[X]M in [Y] years
- **Penetration rate**: [%]% ([rationale])
- **Time to penetration**: [X] years
- **TAM (Comps)**: $[X]M

**Comparables**:
- [Comp 1]: [brief description]
- [Comp 2]: [brief description]

## Triangulated Results

| Method | TAM | SAM | SOM (24mo) |
|--------|-----|-----|------------|
| Bottoms-up | $[X]M | $[Y]M | $[Z]M |
| Tops-down | $[X]M | $[Y]M | $[Z]M |
| Comps | $[X]M | $[Y]M | $[Z]M |
| **Consensus** | **$[X]M** | **$[Y]M** | **$[Z]M** |

## Sensitivity Bands (Min/Base/Max)

| Metric | Min | Base | Max |
|--------|-----|------|-----|
| TAM | $[X]M | $[Y]M | $[Z]M |
| SAM | $[X]M | $[Y]M | $[Z]M |
| SOM (24mo) | $[X]M | $[Y]M | $[Z]M |

## Device Sales vs Service/Recurring

**Device sales component**: $[X]M ([%]% of TAM)
**Service/recurring component**: $[Y]M ([%]% of TAM)

## SOM Path (Next 24 Months)

**Capacity constraints**:
- [Constraint 1]: limits to [X] units/month
- [Constraint 2]: limits to $[Y]M ARR

**Channel constraints**:
- [Channel 1]: can deliver $[X]M
- [Channel 2]: can deliver $[Y]M

**Realistic SOM (24mo)**: $[Z]M

## Sources & Citations
1. [Source 1]: [Description] ([link])
2. [Source 2]: [Description] ([link])
3. [Source 3]: [Description] ([link])

## Red Flags / Common Mistakes Check
- [ ] TAM has clear path to SAM and SOM
- [ ] Channel and capacity constraints explicitly modeled
- [ ] Assumptions stated explicitly with sources
- [ ] Device vs service/recurring split shown
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
