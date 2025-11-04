---
name: Investment Readiness Audit
description: Fast scan for whether this is fundable now, what's missing, and the order of operations.
when_to_use: Before outreach; pre‑IC (investment committee) prep; deck v0.1.
version: 1.0.0
languages: all
---
# Investment Readiness Audit

## Overview
A ruthless checklist to decide **go/no‑go** on fundraising now vs. what to fix first.

## Pre-work (MANDATORY)
1. Read `vc-work/context.md` to understand accumulated context
2. Ask user for current company status across all dimensions (vision, traction, unit econ, market, moat, team, funding) → append to `context.md`
3. Log session start in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`

## Core Questions
- Vision → Why now? What wedge? Category narrative in one sentence?
- Evidence → What traction signals exist (revenue, pilots, LOIs, usage, LTV/CAC)?
- Unit economics → Proved on a *single* SKU/segment yet? Gross margin path?
- Market → Credible bottoms‑up TAM? Who *buys* and why budget exists?
- Moat → Switching costs, data scale, workflow lock‑in, standards/IP?
- Team → Founder‑market fit; can this team ship *this* plan?
- Funding → Milestone plan tied to use of funds; runway math clear?

## Quick Reference (Pass/Fail Signals)
- **Green**: Repeatable pilot→paid conversions; crisp ICP; margin math believable.
- **Yellow**: Anecdotes > data; unclear payback; TAM hand‑wavy.
- **Red**: No painkiller; no buyer; hardware margin < 30% with no path.

## Artifacts
- 1‑page “Why now / What’s different / Proof so far”.
- Milestone‑based use‑of‑funds table (quarters, hires, deliverables, KPIs).

## Common Mistakes
- Leading with tech, burying the buyer and budget.
- Listing features instead of proof.

## MANDATORY Output

**Always create/update**: `vc-work/outputs/investment-readiness-audit-[company].md`

**Format**:
```markdown
# Investment Readiness Audit: [Company Name]
**Date**: YYYY-MM-DD

## Input Data
[Paste of user's current company status from context.md]

## Go/No-Go Assessment

**Overall verdict**: [ ] GREEN (ready to raise) [ ] YELLOW (fixable gaps) [ ] RED (not ready, need milestones first)

**Recommendation**: [Go now / Fix X, Y, Z first / Wait for milestone M]

---

## Dimension-by-Dimension Audit

### 1. Vision (Why Now / What Wedge / Category)

**Category narrative (one sentence)**: [What category are you defining/winning?]

| Question | Answer | Status | Notes |
|----------|--------|--------|-------|
| **Why now?** | [Market shift, regulation, tech unlock] | [ ] Green [ ] Yellow [ ] Red | [What's missing] |
| **What wedge?** | [Initial beachhead, then expand to...] | [ ] Green [ ] Yellow [ ] Red | [What's missing] |
| **Category clarity?** | [Can explain in one sentence] | [ ] Green [ ] Yellow [ ] Red | [What's missing] |

**Red flags**:
- [ ] Leading with tech, not buyer/budget
- [ ] No clear "why now" moment
- [ ] Can't articulate category in one sentence

---

### 2. Evidence (Traction Signals)

| Signal | Current State | Target for Fundability | Status | Notes |
|--------|---------------|----------------------|--------|-------|
| **Revenue** | $[X]K ARR | [Target for round] | [ ] Green [ ] Yellow [ ] Red | [Gap analysis] |
| **Pilots** | [#] active | [# needed] | [ ] Green [ ] Yellow [ ] Red | [Conversion rate] |
| **LOIs** | [#] signed | [# needed] | [ ] Green [ ] Yellow [ ] Red | [Strength of LOIs] |
| **Usage** | [Metric] | [Target] | [ ] Green [ ] Yellow [ ] Red | [Engagement depth] |
| **LTV/CAC** | [Ratio] | >3:1 | [ ] Green [ ] Yellow [ ] Red | [Math shown] |

**Red flags**:
- [ ] Anecdotes > data
- [ ] No repeatable pilot→paid conversions
- [ ] Features listed instead of proof

---

### 3. Unit Economics (Proved on Single SKU/Segment)

| Metric | Current | Target | Status | Notes |
|--------|---------|--------|--------|-------|
| **CAC** | $[X] | <$[Y] | [ ] Green [ ] Yellow [ ] Red | [Payback months] |
| **COGS** | $[X] | <$[Y] | [ ] Green [ ] Yellow [ ] Red | [Gross margin %] |
| **Gross margin** | [%]% | >[%]% | [ ] Green [ ] Yellow [ ] Red | [Path shown] |
| **LTV** | $[X] | >$[Y] | [ ] Green [ ] Yellow [ ] Red | [Retention rate] |
| **LTV:CAC** | [Ratio] | >3:1 | [ ] Green [ ] Yellow [ ] Red | [Believable?] |

**Gross margin path** (8 quarters): [ ] Shown [ ] Not shown

**Red flags**:
- [ ] Unit econ unclear or hand-wavy
- [ ] Payback >24 months with no path to improvement
- [ ] Hardware margin <30% with no credible path to 40%+

---

### 4. Market (TAM Credibility + Buyer Budget)

| Question | Answer | Status | Notes |
|----------|--------|--------|-------|
| **Bottoms-up TAM** | $[X]M | [ ] Green [ ] Yellow [ ] Red | [Calculation shown] |
| **Who buys?** | [Title/role] | [ ] Green [ ] Yellow [ ] Red | [Budget authority clear?] |
| **Why budget exists?** | [KPI they improve, cost they avoid] | [ ] Green [ ] Yellow [ ] Red | [Compelling?] |
| **TAM sources** | [Cited sources] | [ ] Green [ ] Yellow [ ] Red | [Credible?] |

**Red flags**:
- [ ] TAM hand-wavy (no bottoms-up calc)
- [ ] Can't name who writes the check
- [ ] No clear budget rationale beyond "it's better"

---

### 5. Moat (Defensibility)

| Source | Current State | Status | Notes |
|--------|---------------|--------|-------|
| **Data advantage** | [Scale: X records/deployments] | [ ] Green [ ] Yellow [ ] Red | [Compounding shown?] |
| **Workflow lock-in** | [Integration depth] | [ ] Green [ ] Yellow [ ] Red | [Switching cost?] |
| **Standards/IP** | [Filed/granted, adoption] | [ ] Green [ ] Yellow [ ] Red | [Usage scale?] |
| **Distribution** | [Channel density] | [ ] Green [ ] Yellow [ ] Red | [Exclusive?] |
| **Brand** | [Category leadership] | [ ] Green [ ] Yellow [ ] Red | [Mind share?] |

**Red flags**:
- [ ] "First-mover" without usage/data scale
- [ ] "IP filed" without enforcement budget or usage
- [ ] No switching costs or compounding effects

---

### 6. Team (Founder-Market Fit + Ability to Ship)

| Question | Answer | Status | Notes |
|----------|--------|--------|-------|
| **Founder-market fit** | [Why this team, this problem] | [ ] Green [ ] Yellow [ ] Red | [Compelling story?] |
| **Domain expertise** | [Years in space, previous exits] | [ ] Green [ ] Yellow [ ] Red | [Credible?] |
| **Can ship this plan?** | [Track record, key hires] | [ ] Green [ ] Yellow [ ] Red | [Gaps in team?] |
| **Key hires identified** | [Roles needed for this round] | [ ] Green [ ] Yellow [ ] Red | [Realistic?] |

**Red flags**:
- [ ] No relevant domain expertise
- [ ] Can't articulate why this team can win
- [ ] Critical roles unfilled with no plan to fill

---

### 7. Funding (Milestone Plan + Runway Math)

| Question | Answer | Status | Notes |
|----------|--------|--------|-------|
| **Round size** | $[X]M | [ ] Green [ ] Yellow [ ] Red | [Right-sized?] |
| **3 milestones** | [List 3 key milestones] | [ ] Green [ ] Yellow [ ] Red | [Tied to use of funds?] |
| **Runway** | [X] months | [ ] Green [ ] Yellow [ ] Red | [18-24 mo target] |
| **Use of funds** | [% breakdown by function] | [ ] Green [ ] Yellow [ ] Red | [Tied to milestones?] |
| **Burn rate** | $[X]K/month | [ ] Green [ ] Yellow [ ] Red | [Realistic?] |

**Red flags**:
- [ ] Milestones not tied to use of funds
- [ ] Runway math unclear
- [ ] Hiring outpaces GTM capacity

---

## Summary Scorecard

| Dimension | Score | Blockers | Fix-by Date |
|-----------|-------|----------|-------------|
| **Vision** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |
| **Evidence** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |
| **Unit Economics** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |
| **Market** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |
| **Moat** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |
| **Team** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |
| **Funding** | [ ] Green [ ] Yellow [ ] Red | [List blockers] | [Date] |

---

## Order of Operations (What to Fix First)

**P0 (Must fix before any outreach)**:
1. [Blocker 1]: [What to do, who owns it, by when]
2. [Blocker 2]: [What to do, who owns it, by when]
3. [Blocker 3]: [What to do, who owns it, by when]

**P1 (Fix before partner meetings)**:
1. [Gap 1]: [What to do, who owns it, by when]
2. [Gap 2]: [What to do, who owns it, by when]

**P2 (Nice to have)**:
1. [Enhancement 1]: [What to do, who owns it, by when]

---

## One-Pager: "Why Now / What's Different / Proof So Far"

**Why Now** (1-2 sentences):
[Market shift, regulation change, technology unlock, crisis moment that creates the window]

**What's Different** (1-2 sentences):
[Your unique insight, wedge, or approach that others don't have]

**Proof So Far** (3 bullets):
- [Traction metric 1 with number]
- [Traction metric 2 with number]
- [Traction metric 3 with number]

---

## Milestone-Based Use of Funds

| Quarter | Milestone | Owner | Deliverables | KPI | $ Allocated |
|---------|-----------|-------|--------------|-----|-------------|
| Q1 | [Milestone 1] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q2 | [Milestone 2] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q3 | [Milestone 3] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |
| Q4 | [Milestone 4] | [Name] | [What gets built/shipped] | [Success metric] | $[X]K |

---

## Red Flags / Common Mistakes Check
- [ ] NOT leading with tech, buyer and budget clear
- [ ] Proof shown with numbers, not just features
- [ ] Unit economics crisp and believable
- [ ] TAM has credible bottoms-up calculation
- [ ] Moat more than "first-mover" or "IP filed"
- [ ] Team can credibly ship this plan
- [ ] Milestones tied to use of funds with KPIs
```

**End-of-session**: Log summary in `vc-work/session-logs/YYYY-MM-DD-HH-MM.md`
