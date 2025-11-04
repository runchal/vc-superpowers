---
name: Use of Funds & Operating Plan
description: Tie budget to milestones, hires, and de‑risking steps.
when_to_use: Always when mentioning an "ask."
version: 1.0.0
languages: all
---
# Use of Funds & Operating Plan

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for fundraising ask, milestones, and hiring plan → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- What are the **three** milestones this capital unlocks?
- Hiring plan per quarter; burn by function; runway months at Base case.
- Back‑off plan if fundraising slips; contingency triggers.

## Artifacts
- Table: quarter × milestone × owner × KPI × $.

## Common Mistakes
- Buckets without owners; hiring that outpaces GTM capacity.

## MANDATORY Output

**Always create/update**: `vc-work/outputs/use-of-funds-operating-plan-[round].md`

**Format**:
```markdown
# Use of Funds & Operating Plan: [Round Name]
**Date**: YYYY-MM-DD

## Input Data
[Paste of user's fundraising ask and plan from context.md]

## The Ask

**Round size**: $[X]M
**Instrument**: [SAFE / Priced round / Convertible note]
**Key terms**: [Valuation cap, discount, etc.]
**Target close date**: [Date]
**Status**: $[Y]M committed, $[Z]M to raise

## Three Milestones This Capital Unlocks

### Milestone 1: [Name]
**Target**: [Specific metric, e.g., "$2M ARR"]
**Timeline**: [Quarter/Month]
**Owner**: [Name/role]
**Why this matters**: [How this unlocks next round or key inflection point]

### Milestone 2: [Name]
**Target**: [Specific metric]
**Timeline**: [Quarter/Month]
**Owner**: [Name/role]
**Why this matters**: [How this unlocks next round or key inflection point]

### Milestone 3: [Name]
**Target**: [Specific metric]
**Timeline**: [Quarter/Month]
**Owner**: [Name/role]
**Why this matters**: [How this unlocks next round or key inflection point]

## Quarterly Operating Plan

| Quarter | Milestone | Owner | Deliverables | KPI | $ Allocated |
|---------|-----------|-------|--------------|-----|-------------|
| Q1 | [Milestone name] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q2 | [Milestone name] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q3 | [Milestone name] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q4 | [Milestone name] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q5 | [Milestone name] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q6 | [Milestone name] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |

## Hiring Plan by Function

### Engineering

| Quarter | Role | Count | Comp (avg) | Total Cost | What They Enable |
|---------|------|-------|------------|------------|------------------|
| Q1 | [e.g., Senior Engineer] | [#] | $[X]K | $[Y]K | [e.g., V2 launch] |
| Q2 | [e.g., Staff Engineer] | [#] | $[X]K | $[Y]K | [e.g., Scale features] |
| Q3 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q4 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |

**Engineering total**: [#] hires, $[X]K

### Sales & GTM

| Quarter | Role | Count | Comp (avg) | Total Cost | What They Enable |
|---------|------|-------|------------|------------|------------------|
| Q1 | [e.g., VP Sales] | [#] | $[X]K | $[Y]K | [e.g., Build sales process] |
| Q2 | [e.g., AE] | [#] | $[X]K | $[Y]K | [e.g., Scale pipeline] |
| Q3 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q4 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |

**Sales/GTM total**: [#] hires, $[X]K

### Customer Success & Support

| Quarter | Role | Count | Comp (avg) | Total Cost | What They Enable |
|---------|------|-------|------------|------------|------------------|
| Q1 | [e.g., CSM] | [#] | $[X]K | $[Y]K | [e.g., Onboard customers] |
| Q2 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q3 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q4 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |

**CS/Support total**: [#] hires, $[X]K

### Operations

| Quarter | Role | Count | Comp (avg) | Total Cost | What They Enable |
|---------|------|-------|------------|------------|------------------|
| Q1 | [e.g., Operations Manager] | [#] | $[X]K | $[Y]K | [e.g., Supply chain] |
| Q2 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q3 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q4 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |

**Operations total**: [#] hires, $[X]K

### Other (Marketing, Finance, HR, etc.)

| Quarter | Role | Count | Comp (avg) | Total Cost | What They Enable |
|---------|------|-------|------------|------------|------------------|
| Q1 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q2 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q3 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |
| Q4 | [Role] | [#] | $[X]K | $[Y]K | [What they enable] |

**Other total**: [#] hires, $[X]K

### Hiring Summary

| Function | Total Hires | Total Cost | % of Total |
|----------|-------------|------------|------------|
| Engineering | [#] | $[X]K | [%]% |
| Sales/GTM | [#] | $[X]K | [%]% |
| CS/Support | [#] | $[X]K | [%]% |
| Operations | [#] | $[X]K | [%]% |
| Other | [#] | $[X]K | [%]% |
| **Total** | **[#]** | **$[X]K** | **100%** |

## Burn by Function

| Function | Q1 | Q2 | Q3 | Q4 | Q5 | Q6 | Total |
|----------|----|----|----|----|----|----|-------|
| **Engineering** | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K |
| **Sales/GTM** | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K |
| **CS/Support** | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K |
| **Operations** | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K |
| **Other** | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K |
| **Non-headcount** | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K | $[X]K |
| **Total burn** | **$[X]K** | **$[X]K** | **$[X]K** | **$[X]K** | **$[X]K** | **$[X]K** | **$[X]K** |

**Non-headcount breakdown**:
- Cloud/hosting: $[X]K
- Marketing/advertising: $[X]K
- Tools/software: $[X]K
- Office/facilities: $[X]K
- Legal/accounting: $[X]K
- Other: $[X]K

## Runway Analysis

### Base Case

**Total raise**: $[X]M
**Opening balance**: $[Y]K (current cash)
**Total available**: $[Z]M

| Quarter | Starting Cash | Burn | Ending Cash | Runway (Months) |
|---------|--------------|------|-------------|-----------------|
| Q1 | $[X]M | $[Y]K | $[Z]M | [X] |
| Q2 | $[X]M | $[Y]K | $[Z]M | [X] |
| Q3 | $[X]M | $[Y]K | $[Z]M | [X] |
| Q4 | $[X]M | $[Y]K | $[Z]M | [X] |
| Q5 | $[X]M | $[Y]K | $[Z]M | [X] |
| Q6 | $[X]M | $[Y]K | $[Z]M | [X] |

**Runway at Base case burn**: [X] months (target: 18-24 months)

### High Case (Revenue Accelerates)

**Assumptions**: [What drives higher revenue]

| Quarter | Starting Cash | Burn | Revenue | Net Burn | Ending Cash | Runway |
|---------|--------------|------|---------|----------|-------------|--------|
| Q1 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |
| Q2 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |
| Q3 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |
| Q4 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |

**Runway at High case**: [X] months

### Low Case (Slower Growth)

**Assumptions**: [What drives slower growth]

| Quarter | Starting Cash | Burn | Revenue | Net Burn | Ending Cash | Runway |
|---------|--------------|------|---------|----------|-------------|--------|
| Q1 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |
| Q2 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |
| Q3 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |
| Q4 | $[X]M | $[Y]K | $[R]K | $[N]K | $[Z]M | [X] |

**Runway at Low case**: [X] months

## Back-Off Plan (If Fundraising Slips)

**Trigger**: If round not closed by [date], activate back-off plan

### Cost Reduction Levers

| Lever | Savings/Quarter | Impact on Milestones |
|-------|-----------------|---------------------|
| [e.g., Delay 2 eng hires] | $[X]K | [Impact: V2 launch delayed 1 quarter] |
| [e.g., Cut marketing spend] | $[Y]K | [Impact: Slower pipeline growth] |
| [e.g., Freeze non-critical hires] | $[Z]K | [Impact: Minimal] |
| **Total savings** | **$[X]K** | |

**Extended runway with back-off**: [X] months (from [Y] months)

### Contingency Triggers

**Tripwire 1**: If cash < $[X]K by [date], activate [action]
**Tripwire 2**: If fundraising not closed by [date], activate [action]
**Tripwire 3**: If burn > $[Y]K/month for 2 consecutive months, activate [action]

## GTM Capacity Check

**Sales capacity** (can hiring support growth plan?):

| Quarter | # AEs | Quota/AE | Total Capacity | Revenue Target | Utilization |
|---------|-------|----------|----------------|----------------|-------------|
| Q1 | [#] | $[X]K | $[Y]K | $[Z]K | [%]% |
| Q2 | [#] | $[X]K | $[Y]K | $[Z]K | [%]% |
| Q3 | [#] | $[X]K | $[Y]K | $[Z]K | [%]% |
| Q4 | [#] | $[X]K | $[Y]K | $[Z]K | [%]% |

**Red flag**: If utilization > 100%, hiring is behind GTM plan

## Use of Funds Summary Table

| Category | Amount | % of Total | Milestones Enabled |
|----------|--------|------------|--------------------|
| **Engineering** | $[X]K | [%]% | [Milestone 1, 2] |
| **Sales/GTM** | $[X]K | [%]% | [Milestone 1, 3] |
| **CS/Support** | $[X]K | [%]% | [Milestone 2] |
| **Operations** | $[X]K | [%]% | [Milestone 1] |
| **Marketing** | $[X]K | [%]% | [Milestone 3] |
| **Other** | $[X]K | [%]% | [General operations] |
| **Total** | **$[X]M** | **100%** | |

## Red Flags / Common Mistakes Check
- [ ] Every bucket has an owner (not just "Engineering: $X")
- [ ] Hiring does NOT outpace GTM capacity (sales hiring supports revenue plan)
- [ ] Milestones explicitly tied to use of funds
- [ ] Runway math clear (18-24 months target)
- [ ] Back-off plan exists with specific triggers
- [ ] Contingency triggers defined (not just "we'll figure it out")
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
