---
name: Regulatory & Certification (Deeptech/Hardware)
description: Map required approvals (UL/IEC, FCC/CE, DOT/FAA), timelines, and costs.
when_to_use: Any hardware, energy, or regulated deployment.
version: 1.0.0
languages: all
---
# Regulatory & Certification (Deeptech/Hardware)

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for regulatory/certification data (product type, target markets, required certs) → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- Which standards apply (UL 9540/1973/1741, IEC, NFPA, NEC)?
- Testing plan: pre‑compliance, lab slots, redesign risks, costs.
- Site approvals: AHJ (authority having jurisdiction), permits, interconnects.
- Safety, warranty, and liability assumptions.

## Artifacts
- Certification map with dates/costs; block‑and‑tackle for AHJs.

## Common Mistakes
- Treating certs as paperwork instead of design constraints.

## MANDATORY Output

**Always create/update**: `vc-work/outputs/regulatory-and-certification-[product].md`

**Format**:
```markdown
# Regulatory & Certification: [Product Name]
**Date**: YYYY-MM-DD

## Input Data
[Paste of user's regulatory/certification data from context.md]

## Standards Roadmap

### Required Standards (By Market)

**US Market**:
- [ ] **UL [standard #]**: [e.g., UL 9540 for BESS]
- [ ] **FCC Part [X]**: [e.g., Part 15 for RF emissions]
- [ ] **NEC [article]**: [e.g., Article 706 for energy storage]
- [ ] **NFPA [code]**: [e.g., NFPA 855 for BESS installations]
- [ ] **Other**: [OSHA, EPA, DOT, etc.]

**EU Market**:
- [ ] **CE Mark**: [Directives: LVD, EMC, RED, etc.]
- [ ] **IEC [standard #]**: [e.g., IEC 62619 for batteries]
- [ ] **EN [standard #]**: [e.g., EN 50598 for power drive systems]
- [ ] **Other**: [REACH, RoHS, WEEE, etc.]

**Other Markets**:
- [ ] **Canada**: [CSA standards]
- [ ] **Asia**: [CCC (China), PSE (Japan), KC (Korea)]
- [ ] **Australia**: [AS/NZS standards]

### Standards by Priority

| Standard | Market | Priority | Required for Launch? | Timeline | Cost | Status |
|----------|--------|----------|---------------------|----------|------|--------|
| [e.g., UL 9540] | US | P0 | Yes | [X] months | $[X]K | [ ] Not started [ ] In progress [ ] Complete |
| [e.g., FCC Part 15] | US | P0 | Yes | [X] months | $[X]K | [ ] Not started [ ] In progress [ ] Complete |
| [e.g., CE Mark] | EU | P1 | No (for v1) | [X] months | $[X]K | [ ] Not started [ ] In progress [ ] Complete |
| [e.g., IEC 62619] | EU | P1 | No (for v1) | [X] months | $[X]K | [ ] Not started [ ] In progress [ ] Complete |

## Testing Plan

### Pre-Compliance Testing

**Purpose**: Identify issues before expensive formal testing

| Test | Vendor/Lab | Cost | Timeline | Status | Results |
|------|------------|------|----------|--------|---------|
| [e.g., EMC pre-scan] | [Vendor] | $[X]K | [X] weeks | [ ] Not started [ ] In progress [ ] Complete | [Pass/Fail, issues found] |
| [e.g., Safety review] | [Vendor] | $[X]K | [X] weeks | [ ] Not started [ ] In progress [ ] Complete | [Pass/Fail, issues found] |
| [e.g., Thermal testing] | [Vendor] | $[X]K | [X] weeks | [ ] Not started [ ] In progress [ ] Complete | [Pass/Fail, issues found] |

### Formal Certification Testing

**Lab selection**: [Name of test lab(s)]
**Lab slots booked**: [ ] Yes [ ] No (target date: [date])

| Certification | Lab | Test Duration | Lead Time to Book | Cost | Status |
|---------------|-----|---------------|------------------|------|--------|
| [e.g., UL 9540] | [Lab name] | [X] weeks | [Y] weeks | $[X]K | [ ] Not booked [ ] Booked [ ] Testing [ ] Complete |
| [e.g., FCC] | [Lab name] | [X] weeks | [Y] weeks | $[X]K | [ ] Not booked [ ] Booked [ ] Testing [ ] Complete |
| [e.g., CE] | [Lab name] | [X] weeks | [Y] weeks | $[X]K | [ ] Not booked [ ] Booked [ ] Testing [ ] Complete |

### Redesign Risk Budget

**Probability of redesign**: [Low / Medium / High]

**Redesign scenarios**:
1. **[Scenario 1: e.g., EMC failure]**:
   - **Probability**: [%]%
   - **Cost**: $[X]K
   - **Time delay**: [X] months
   - **Mitigation**: [Pre-compliance testing, design review]

2. **[Scenario 2: e.g., Safety issue]**:
   - **Probability**: [%]%
   - **Cost**: $[X]K
   - **Time delay**: [X] months
   - **Mitigation**: [Early prototype testing, expert review]

3. **[Scenario 3: e.g., Thermal failure]**:
   - **Probability**: [%]%
   - **Cost**: $[X]K
   - **Time delay**: [X] months
   - **Mitigation**: [Simulation, component selection]

**Total redesign contingency**: $[X]K ([sum of weighted scenarios])

## Site Approvals

### Authority Having Jurisdiction (AHJ) Process

**Typical AHJs** (for our deployments):
- **[AHJ type 1: e.g., Fire Marshal]**: [Requirements, typical timeline]
- **[AHJ type 2: e.g., Building Dept]**: [Requirements, typical timeline]
- **[AHJ type 3: e.g., Utility]**: [Requirements, typical timeline]

### Permits Required (Per Deployment)

| Permit Type | Issuing Authority | Documents Required | Timeline | Cost | Variability |
|-------------|-------------------|-------------------|----------|------|-------------|
| [e.g., Building permit] | [City/county] | [Plans, calcs, certs] | [X] weeks | $[X] | [Low/Med/High] |
| [e.g., Electrical permit] | [City/county] | [Plans, calcs, certs] | [X] weeks | $[X] | [Low/Med/High] |
| [e.g., Fire permit] | [Fire dept] | [Plans, calcs, certs] | [X] weeks | $[X] | [Low/Med/High] |
| [e.g., Environmental] | [EPA/state] | [Plans, calcs, certs] | [X] weeks | $[X] | [Low/Med/High] |

### Interconnection (If Applicable)

**Utility interconnection process**:
- **Application**: [Documents required, timeline, cost]
- **Study**: [Impact study, timeline, cost]
- **Agreement**: [Standard agreement vs custom, timeline]
- **Typical total timeline**: [X] months
- **Typical total cost**: $[X]

**Block-and-tackle plan for AHJs**:
1. [Step 1: e.g., Identify all required permits in advance]
2. [Step 2: e.g., Pre-submit plans for informal review]
3. [Step 3: e.g., Build relationship with inspectors]
4. [Step 4: e.g., Track approval timelines by jurisdiction]

## Design Constraints from Certifications

**How certifications impact design**:

| Certification | Design Constraint | Impact on Product | Mitigation |
|---------------|------------------|-------------------|------------|
| [e.g., UL 9540] | [e.g., Specific fire suppression] | [Cost: +$X/unit] | [Design in from start] |
| [e.g., FCC Part 15] | [e.g., RF shielding requirements] | [Cost: +$X/unit, Weight: +Y kg] | [Early EMC testing] |
| [e.g., NEC Article 706] | [e.g., Specific disconnect requirements] | [BOM change: $X] | [Consult with AHJs early] |
| [e.g., CE/IEC] | [e.g., Different voltage/frequency] | [Design variants needed] | [Modular power supply] |

**Critical design decisions driven by certs**:
1. [Decision 1]: [How cert shaped the design]
2. [Decision 2]: [How cert shaped the design]
3. [Decision 3]: [How cert shaped the design]

## Safety, Warranty, and Liability

### Safety Assumptions

**Failure modes addressed**:
1. [Failure mode 1]: [How mitigated, what standard requires it]
2. [Failure mode 2]: [How mitigated, what standard requires it]
3. [Failure mode 3]: [How mitigated, what standard requires it]

**Safety-critical components**:
- [Component 1]: [Vendor, cert, backup supplier]
- [Component 2]: [Vendor, cert, backup supplier]
- [Component 3]: [Vendor, cert, backup supplier]

### Warranty Terms

**Standard warranty**: [X] years
**Extended warranty** (optional): [Y] years (+$[Z])

**What's covered**:
- [Coverage 1]
- [Coverage 2]
- [Coverage 3]

**What's excluded**:
- [Exclusion 1]
- [Exclusion 2]

### Liability & Insurance

**Product liability insurance**: $[X]M coverage
**Cost**: $[Y]K/year
**Deductible**: $[Z]K

**Key exclusions**: [What's not covered]

## Certification Timeline & Cost Summary

### Timeline (Gantt Chart)

| Quarter | Q1 | Q2 | Q3 | Q4 | Q5 | Q6 |
|---------|----|----|----|----|----|----|
| **Pre-compliance** | [X] | [X] | | | | |
| **Design freeze** | | [X] | | | | |
| **Formal testing** | | | [X] | [X] | | |
| **Cert received** | | | | [X] | | |
| **First deployment** | | | | | [X] | |

### Cost Summary

| Category | Cost | Notes |
|----------|------|-------|
| **Pre-compliance testing** | $[X]K | [Lab fees, travel] |
| **Formal certifications** | $[Y]K | [All required certs] |
| **Redesign contingency** | $[Z]K | [Weighted probability] |
| **Legal/consulting** | $[A]K | [Expert reviews, regulatory counsel] |
| **Permits (per site)** | $[B]K | [Avg cost per deployment] |
| **Insurance (annual)** | $[C]K | [Product liability] |
| **Total (first year)** | **$[Total]K** | |
| **Ongoing (annual)** | **$[C]K** | [Insurance + audit costs] |

## Red Flags / Common Mistakes Check
- [ ] Certifications treated as design constraints, not just paperwork
- [ ] Redesign risk budgeted (time and cost)
- [ ] Lab slots booked or timeline to book clear
- [ ] AHJ process mapped out (not assuming "just submit plans")
- [ ] Safety assumptions explicit (failure modes addressed)
- [ ] Permit variability by jurisdiction understood
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
