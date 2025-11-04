---
name: Risk Matrix & Mitigations
description: Make risks explicit and show how you burn them down.
when_to_use: Any time investors will ask "what could kill this?"
version: 1.0.0
languages: all
---
# Risk Matrix & Mitigations

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for known risks and concerns → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- Risks by category: market, technical, regulatory, supply chain, capital.
- Mitigations: experiments, partnerships, insurance, design changes.
- Tripwires: metrics that trigger plan B.

## Artifacts
- R×I (risk × impact) heatmap; burn‑down timeline.

## Common Mistakes
- Hiding obvious risks (certifications, gross margin, channel power).

## MANDATORY Output

**Always create/update**: `vc-work/outputs/risk-matrix-and-mitigations-[company].md`

**Format**:
```markdown
# Risk Matrix & Mitigations: [Company Name]
**Date**: YYYY-MM-DD

## Input Data
[Paste of user's known risks from context.md]

## Risk Categories

### Market Risks

| Risk | Probability | Impact | R×I Score | Current Status | Mitigation | Tripwire |
|------|-------------|--------|-----------|----------------|------------|----------|
| [e.g., TAM smaller than expected] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Customer adoption slower] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Competitor enters market] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |

### Technical Risks

| Risk | Probability | Impact | R×I Score | Current Status | Mitigation | Tripwire |
|------|-------------|--------|-----------|----------------|------------|----------|
| [e.g., Product doesn't meet spec] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Integration more complex] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Scaling challenges] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |

### Regulatory Risks

| Risk | Probability | Impact | R×I Score | Current Status | Mitigation | Tripwire |
|------|-------------|--------|-----------|----------------|------------|----------|
| [e.g., Certification delayed] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Standard changes] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., AHJ rejects design] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |

### Supply Chain Risks

| Risk | Probability | Impact | R×I Score | Current Status | Mitigation | Tripwire |
|------|-------------|--------|-----------|----------------|------------|----------|
| [e.g., Component shortage] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Single-source vendor] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Cost escalation] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |

### Capital Risks

| Risk | Probability | Impact | R×I Score | Current Status | Mitigation | Tripwire |
|------|-------------|--------|-----------|----------------|------------|----------|
| [e.g., Fundraising takes longer] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Bridge round needed] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Burn exceeds plan] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |

### Other Risks

| Risk | Category | Probability | Impact | R×I Score | Current Status | Mitigation | Tripwire |
|------|----------|-------------|--------|-----------|----------------|------------|----------|
| [e.g., Key hire doesn't join] | [People] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Channel partner conflict] | [GTM] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |
| [e.g., Gross margin compression] | [Financial] | [L/M/H] | [L/M/H] | [#] | [Red/Yellow/Green] | [Mitigation plan] | [Metric that triggers plan B] |

**Scoring**:
- Probability: Low (1), Medium (2), High (3)
- Impact: Low (1), Medium (2), High (3)
- R×I Score: Probability × Impact (1-9)

## Risk Heatmap

**High Impact, High Probability (R×I = 6-9)** - TOP PRIORITY:
1. [Risk name]: [Mitigation]
2. [Risk name]: [Mitigation]
3. [Risk name]: [Mitigation]

**High Impact, Medium Probability (R×I = 4-6)** - MONITOR:
1. [Risk name]: [Mitigation]
2. [Risk name]: [Mitigation]

**Medium Impact, High Probability (R×I = 4-6)** - MONITOR:
1. [Risk name]: [Mitigation]
2. [Risk name]: [Mitigation]

**Low Priority (R×I = 1-3)** - ACKNOWLEDGE:
[List low-priority risks]

## Mitigation Plans (Detailed)

### Risk 1: [Name of highest R×I risk]

**Category**: [Market/Technical/Regulatory/Supply Chain/Capital]
**Probability**: [L/M/H] ([%]%)
**Impact**: [L/M/H] ([$X] or [Y] month delay)
**R×I Score**: [#]

**Why this is a risk**:
[Explanation of what could go wrong and why it matters]

**Mitigation approaches**:
1. **[Approach 1]**: [What we're doing to reduce probability or impact]
   - **Owner**: [Name]
   - **Timeline**: [By when]
   - **Cost**: $[X]
   - **Success metric**: [How we know it's working]

2. **[Approach 2]**: [Alternative approach or backup plan]
   - **Owner**: [Name]
   - **Timeline**: [By when]
   - **Cost**: $[X]
   - **Success metric**: [How we know it's working]

**Tripwire** (what triggers plan B):
[Specific metric or event that signals we need to pivot]
- If [metric] < [threshold] by [date], then [action]

**Plan B**:
[What we do if mitigation fails or tripwire is triggered]

---

### Risk 2: [Name of second highest R×I risk]

[Repeat structure above for each high-priority risk]

---

## Risk Burn-Down Timeline

| Quarter | Risk | Mitigation Activity | Success Metric | Target |
|---------|------|---------------------|----------------|--------|
| Q1 | [Risk 1] | [Activity] | [Metric] | [Target value] |
| Q1 | [Risk 2] | [Activity] | [Metric] | [Target value] |
| Q2 | [Risk 1] | [Activity] | [Metric] | [Target value] |
| Q2 | [Risk 3] | [Activity] | [Metric] | [Target value] |
| Q3 | [Risk 2] | [Activity] | [Metric] | [Target value] |
| Q3 | [Risk 4] | [Activity] | [Metric] | [Target value] |
| Q4 | [Risk 3] | [Activity] | [Metric] | [Target value] |

**Visual**: [Show how R×I scores decrease over time as mitigations take effect]

## Partnerships, Insurance, and Design Changes

### Partnerships (to share/transfer risk)

| Risk | Partner | How Partnership Mitigates | Terms |
|------|---------|---------------------------|-------|
| [e.g., Supply chain] | [Vendor name] | [Co-development agreement, volume commitment] | [Key terms] |
| [e.g., Regulatory] | [Lab/consultant] | [Pre-compliance testing, design review] | [Key terms] |
| [e.g., Market] | [Channel partner] | [Co-marketing, lead sharing] | [Key terms] |

### Insurance (to transfer risk)

| Risk | Insurance Type | Coverage | Cost | Deductible |
|------|---------------|----------|------|------------|
| [e.g., Product liability] | [Product liability] | $[X]M | $[Y]K/year | $[Z]K |
| [e.g., Key person] | [Key person insurance] | $[X]M | $[Y]K/year | N/A |
| [e.g., D&O] | [Directors & Officers] | $[X]M | $[Y]K/year | $[Z]K |

### Design Changes (to eliminate risk)

| Risk | Design Change | Cost Impact | Timeline Impact | Status |
|------|---------------|-------------|-----------------|--------|
| [e.g., Certification failure] | [Modular design for easier compliance] | +$[X]/unit | +[Y] months | [ ] Planned [ ] In progress [ ] Complete |
| [e.g., Component shortage] | [Dual-source critical components] | +$[X]/unit | +[Y] months | [ ] Planned [ ] In progress [ ] Complete |
| [e.g., Margin compression] | [Redesign for manufacturability] | -$[X]/unit | +[Y] months | [ ] Planned [ ] In progress [ ] Complete |

## Experiments to De-Risk

**Planned experiments** (to reduce uncertainty before committing capital):

| Risk | Experiment | Cost | Timeline | Success Criteria | Go/No-Go Decision |
|------|------------|------|----------|------------------|-------------------|
| [Risk 1] | [Experiment design] | $[X] | [Y] weeks | [Metric > threshold] | [What we decide based on results] |
| [Risk 2] | [Experiment design] | $[X] | [Y] weeks | [Metric > threshold] | [What we decide based on results] |
| [Risk 3] | [Experiment design] | $[X] | [Y] weeks | [Metric > threshold] | [What we decide based on results] |

## Red Flags / Common Mistakes Check
- [ ] Obvious risks NOT hidden (certifications, gross margin, channel power called out)
- [ ] Tripwires defined (not just "we'll monitor")
- [ ] Mitigations specific (not just "work with partners")
- [ ] R×I scores drive priority (not gut feel)
- [ ] Plan B exists for high-impact risks
- [ ] Experiments designed to de-risk before committing capital
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
