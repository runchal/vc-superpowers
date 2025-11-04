---
name: Pricing & Packaging
description: Set initial price, packaging, and discount guardrails linked to value.
when_to_use: Before GTM experiments and before quoting pilots.
version: 1.0.0
languages: all
---
# Pricing & Packaging

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for pricing/packaging data (current pricing, value metric, customer ROI) → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- What metric best tracks value (seat, device, kWh, job, site, SLA)?
- What’s the **price ladder** (Good/Better/Best) and upsell path?
- What discounts exist (pilot, prepay, volume) and floors?
- Hardware + software bundle or separate? Warranty/SLA tiers?

## Quick Reference
- Price test plan: 5 deals, 3 price points, track win rate and payback.
- ROI one‑pager template tied to buyer KPI.

## Artifacts
- Price ladder table; discount policy; ROI calc worksheet.

## Common Mistakes
- Picking a metric you can't meter or invoice cleanly.
- Backing into price from cost instead of value.

## MANDATORY Output

**Always create/update**: `vc-work/outputs/pricing-and-packaging-[product].md`

**Format**:
```markdown
# Pricing & Packaging: [Product/Service Name]
**Date**: YYYY-MM-DD

## Input Data
[Paste of user's pricing/packaging data from context.md]

## Value Metric Selection

**Primary value metric**: [seat / device / kWh / job / site / SLA tier / etc.]

**Why this metric**:
- [ ] **Tracks value**: [How metric correlates with customer value]
- [ ] **Meterable**: [How we measure/track it]
- [ ] **Invoiceable**: [How we bill it cleanly]
- [ ] **Customer understands it**: [How they think about value]

**Alternatives considered**:
1. [Alternative 1]: [Why rejected]
2. [Alternative 2]: [Why rejected]

## Price Ladder (Good/Better/Best)

### Tier 1: [Name, e.g., "Starter"]
**Price**: $[X]/[value metric]/[period]

**Features included**:
- [Feature 1]
- [Feature 2]
- [Feature 3]

**Target customer**: [Who this is for]
**Positioning**: [Why they'd choose this tier]

### Tier 2: [Name, e.g., "Professional"]
**Price**: $[Y]/[value metric]/[period]

**Everything in Tier 1, plus**:
- [Feature 4]
- [Feature 5]
- [Feature 6]

**Target customer**: [Who this is for]
**Positioning**: [Why they'd choose this tier]

### Tier 3: [Name, e.g., "Enterprise"]
**Price**: $[Z]/[value metric]/[period] (or "Custom")

**Everything in Tier 2, plus**:
- [Feature 7]
- [Feature 8]
- [Feature 9]

**Target customer**: [Who this is for]
**Positioning**: [Why they'd choose this tier]

## Upsell Path

**Tier 1 → Tier 2 triggers**:
- [Trigger 1: usage threshold, feature need, etc.]
- [Trigger 2]

**Tier 2 → Tier 3 triggers**:
- [Trigger 1]
- [Trigger 2]

**Expansion drivers** (within tier):
- [Driver 1: more seats, more devices, etc.]
- [Driver 2]

## Discount Policy

### Pilot Discount
**Amount**: [%]% off or $[X] pilot fee
**Duration**: [X] weeks/months
**Conversion pricing**: [What they pay after pilot]
**Floor**: No discount below $[Y]

### Prepay Discount
**12-month prepay**: [%]% off
**24-month prepay**: [%]% off
**36-month prepay**: [%]% off
**Terms**: [Payment terms, refund policy]

### Volume Discount
| Volume (units) | Discount |
|----------------|----------|
| 1-10 | 0% (list price) |
| 11-50 | [%]% |
| 51-100 | [%]% |
| 101+ | [%]% (or custom) |

**Floor**: No discount below $[X]/unit regardless of volume

### Other Discounts
**Education/nonprofit**: [%]% off
**Early adopter**: [%]% off (expires [date])
**Referral**: [%]% off or $[credit]

**Stackability**: [Which discounts can be combined, which can't]

## Hardware + Software Bundling

**Option 1: Bundle**
- **Price**: $[X] (hardware + software subscription)
- **Pros**: [Why customers like this]
- **Cons**: [Why some don't]

**Option 2: Separate**
- **Hardware**: $[Y] one-time
- **Software**: $[Z]/month
- **Pros**: [Why customers like this]
- **Cons**: [Why some don't]

**Recommended approach**: [Bundle / Separate / Offer both] because [rationale]

## Warranty/SLA Tiers

### Basic (included)
**Response time**: [X] hours
**Support channels**: [Email, portal, etc.]
**Uptime guarantee**: [%]%
**Penalty**: [None / Credits / Refund]

### Premium (+$[X]/month or [%]% of contract)
**Response time**: [Y] hours
**Support channels**: [Phone, email, Slack, etc.]
**Uptime guarantee**: [%]%
**Penalty**: [Credits / Refund / SLA credits]

### Enterprise (Custom)
**Response time**: [Z] minutes
**Support channels**: [Dedicated account manager, 24/7 hotline, etc.]
**Uptime guarantee**: [%]%
**Penalty**: [Custom SLA penalties]

## Price Testing Plan

**Test setup**: 5 deals, 3 price points, track win rate and payback

| Price Point | # Deals | Win Rate | Avg Deal Size | Payback (Months) | Notes |
|-------------|---------|----------|---------------|------------------|-------|
| **Low** ($[X]) | [#] | [%]% | $[X] | [X] | [Customer feedback] |
| **Mid** ($[Y]) | [#] | [%]% | $[Y] | [X] | [Customer feedback] |
| **High** ($[Z]) | [#] | [%]% | $[Z] | [X] | [Customer feedback] |

**Learning**: [What we learned, which price point to anchor on]

## ROI Calculation Worksheet

**For [Tier/Package]**:

### Customer's Current State (Baseline)
| Cost/Metric | Annual Amount |
|-------------|---------------|
| [Cost 1: e.g., labor hours] | $[X]/year |
| [Cost 2: e.g., downtime] | $[Y]/year |
| [Cost 3: e.g., waste] | $[Z]/year |
| **Total annual cost** | **$[Total]** |

### With Our Solution
| Cost/Metric | Annual Amount | Savings |
|-------------|---------------|---------|
| [Cost 1 after] | $[X2]/year | $[X - X2] |
| [Cost 2 after] | $[Y2]/year | $[Y - Y2] |
| [Cost 3 after] | $[Z2]/year | $[Z - Z2] |
| **Our price** | -$[Our price] | N/A |
| **Net annual savings** | **$[Net]** | **$[Total savings]** |

**ROI**: [X]% ([Total savings] / [Our price])
**Payback period**: [X] months

### ROI One-Pager Template

```markdown
# ROI Calculator: [Product Name]

**Your current annual cost**: $[X]
**Your cost with [Product]**: $[Y] (including our price)
**Annual savings**: $[Z]
**ROI**: [%]%
**Payback**: [X] months

[Simple table or chart showing before/after]
```

## Price Communication

**Pricing page**: [ ] Public [ ] Gated [ ] Sales-only
**Positioning**: [How we talk about price in context of value]
**Anchoring**: [What we compare to: status quo cost, competitor price, value delivered]

## Red Flags / Common Mistakes Check
- [ ] Value metric is meterable and invoiceable
- [ ] Pricing based on value delivered, not just cost-plus
- [ ] Discount policy has clear floors (no bottomless discounting)
- [ ] ROI calc tied to specific buyer KPI
- [ ] Price ladder has clear upsell path
- [ ] Warranty/SLA tiers match customer needs
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
