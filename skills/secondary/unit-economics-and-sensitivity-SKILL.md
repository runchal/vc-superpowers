---
name: Unit Economics & Sensitivity
description: Build contribution margin and payback with explicit sensitivity bands.
when_to_use: Before setting growth targets or fundraising ask.
version: 1.0.0
languages: all
---
# Unit Economics & Sensitivity

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for current unit economics data (CAC, COGS, pricing, retention) → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- CAC (customer acquisition cost) → blended, by channel; payback months.
- COGS (cost of goods sold) detail: hardware, install, support, hosting.
- Gross margin path over 8 quarters; scale curves (BOM, labor, overhead).
- Retention: logo %, net revenue retention, expansion drivers.

## Quick Reference
- Show Base/Low/High; call out **break‑even** volume explicitly.
- Include learning‑curve step changes (design rev, vendor change, certs).

## Artifacts
- One table per SKU/segment; a simple tornado chart of sensitivities.

## Common Mistakes
- Mixing GAAP and cash metrics; hiding install costs in "one‑time".

## MANDATORY Output

**Always create/update**: `vc-work/outputs/unit-economics-[segment].md`

**Format**:
```markdown
# Unit Economics: [Segment/SKU Name]
**Date**: YYYY-MM-DD

## Input Data
[Paste of user's current unit economics data from context.md]

## Core Metrics

### Customer Acquisition Cost (CAC)
- **Blended CAC**: $[amount]
- **By channel**:
  - [Channel 1]: $[amount]
  - [Channel 2]: $[amount]
- **Payback period**: [X] months

### Cost of Goods Sold (COGS)
- **Hardware**: $[amount] ([%]% of total)
- **Install/labor**: $[amount] ([%]% of total)
- **Support**: $[amount] ([%]% of total)
- **Hosting/cloud**: $[amount] ([%]% of total)
- **Total COGS**: $[amount]

### Gross Margin Path (8 Quarters)
| Quarter | Q1 | Q2 | Q3 | Q4 | Q5 | Q6 | Q7 | Q8 |
|---------|----|----|----|----|----|----|----|----|
| Gross Margin % | [%] | [%] | [%] | [%] | [%] | [%] | [%] | [%] |
| Units Sold | [#] | [#] | [#] | [#] | [#] | [#] | [#] | [#] |

**Scale curve notes**: [BOM reductions, labor efficiency, overhead absorption]

### Retention
- **Logo retention**: [%]%
- **Net revenue retention (NRR)**: [%]%
- **Expansion drivers**: [What drives upsell/expansion?]

## Sensitivity Analysis

### Base / Low / High Scenarios
| Metric | Low | Base | High |
|--------|-----|------|------|
| CAC | $[X] | $[Y] | $[Z] |
| COGS | $[X] | $[Y] | $[Z] |
| Gross Margin | [%]% | [%]% | [%]% |
| Retention | [%]% | [%]% | [%]% |
| **Break-even volume** | [X] units | [Y] units | [Z] units |

### Tornado Chart (Sensitivity Drivers)
[List top 3-5 variables by impact on profitability]
1. [Variable 1]: ±[X]% impact on gross margin
2. [Variable 2]: ±[X]% impact on gross margin
3. [Variable 3]: ±[X]% impact on gross margin

## Learning Curve Step Changes
[Document expected improvements from design revisions, vendor changes, certifications]
- **[Change 1]**: [Expected impact] in [Quarter X]
- **[Change 2]**: [Expected impact] in [Quarter X]

## Red Flags / Common Mistakes Check
- [ ] GAAP vs cash metrics clearly separated
- [ ] Install costs NOT hidden in "one-time"
- [ ] Break-even volume explicitly stated
- [ ] Scale curves show realistic improvement paths
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
