# VC Superpowers - Claude Code Plugin

Transform rough thoughts, emails, and notes into polished, VC-ready content through **Socratic refinement + structured outputs**.

## What It Does

This Claude Code plugin helps founders turn raw ideas into investor-ready materials:

**Input**: Copy/paste thoughts, emails, investor Q&A, rough drafts
**Process**: Socratic questioning → poke holes → refine → structure
**Output**: Markdown files ready to copy/paste into decks, memos, data rooms

## Key Features

- **Context Accumulation**: All your inputs are saved and referenced across sessions
- **Session Logging**: Every session is logged so you can track your progress
- **Structured Outputs**: Every skill produces copy/paste-ready markdown files
- **Auto-Loading**: Primary skills automatically load relevant secondary skills (TAM, unit economics, GTM, etc.)
- **16 Secondary Skills**: Comprehensive coverage of fundraising topics

## Commands

### Primary Workflows (Socratic Flows)

Run these for interactive refinement:

- `/vc:advice` - Advisory flow (Frame → Probe → Options → Recommendation → Commit)
- `/vc:shoot-the-shit` - Free-flow exploration with tiles and parking lot
- `/vc:research` - Generate research plans and query sets (no execution)
- `/vc:stuck` - Unblocker for overcoming friction (15-min micro-plans)
- `/vc:punch-it-up` - Sharpen narratives and pitches with before/after rewrites

### Secondary Skills (Manual Checklists)

Run these for specific checklists:

- `/vc2:tam-sam-som-triangulation` - Market sizing with 3 methods
- `/vc2:unit-economics-and-sensitivity` - Unit economics and sensitivity analysis
- `/vc2:problem-and-customer-pain` - ICP and pain math
- `/vc2:competition-and-positioning` - Competitive analysis
- `/vc2:defensibility-and-barriers` - Moat analysis
- `/vc2:fundraising-narrative-and-arc` - 10-12 slide deck structure
- `/vc2:growth-motion-and-sales-design` - GTM planning
- `/vc2:pricing-and-packaging` - Pricing strategy
- `/vc2:traction-metrics-and-milestones` - KPI tracking
- `/vc2:use-of-funds-and-operating-plan` - Use of funds planning
- `/vc2:investment-readiness-audit` - Fundraise readiness check
- `/vc2:pilots-and-case-studies` - Pilot and case study templates
- `/vc2:risk-matrix-and-mitigations` - Risk analysis
- `/vc2:diligence-data-room-checklist` - Data room organization
- `/vc2:regulatory-and-certification-deeptech` - Regulatory roadmap
- `/vc2:using-vc-skills` - Skills usage log

## Installation

See [INSTALL.md](./INSTALL.md) for detailed instructions.

**Quick start**:

```bash
# Clone to your Claude Code plugins directory
cd ~/.claude/plugins
git clone https://github.com/[your-username]/vc-superpowers.git

# Create vc-work directory (or let Claude create it)
mkdir -p ~/vc-work/session-logs ~/vc-work/outputs
```

Restart Claude Code, and run `/vc:advice` to test.

## Example Workflow

### 1. Start with Rough Investor Q&A

You have a rough email response to an investor asking about unit economics. You want to polish it.

### 2. Run `/vc:punch-it-up`

```
You: /vc:punch-it-up

Claude: I'll help sharpen your narrative. First, let me load context...
[Reads vc-work/context.md]

Paste your current framing/copy:

You: [paste rough investor response]

Claude: [Appends to context.md, auto-loads unit-economics-and-sensitivity skill]

What audience + outcome are you targeting?
[Socratic questions...]
```

### 3. Get Structured Output

Claude creates `vc-work/outputs/punch-it-up-unit-economics.md`:

```markdown
# Punch It Up: Unit Economics Response
**Date**: 2025-11-03

## Before/After Rewrites
### Cold Open
- **Before**: "Our unit economics are good..."
- **After**: "We hit 12-month payback on $1.8K/day battery rentals with 80% gross margin..."

[...complete structured output...]
```

### 4. Copy/Paste into Email

Open `vc-work/outputs/punch-it-up-unit-economics.md`, copy the "After" sections, paste into your investor email. Done.

## How Auto-Loading Works

When you run `/vc:advice` with keywords like "unit economics", "TAM", or "ICP", Claude automatically:

1. Scans your input for keywords
2. Uses the Skill tool to load relevant secondary skills
3. Absorbs the Core Questions and Artifacts from each skill
4. Synthesizes questions across all loaded skills
5. Produces outputs that integrate multiple frameworks

**Example**: You run `/vc:advice` and mention "market sizing" and "payback period"
- Claude auto-loads `tam-sam-som-triangulation` + `unit-economics-and-sensitivity`
- You get questions about bottoms-up/tops-down TAM + CAC/LTV/gross margin
- Output includes both TAM analysis and unit economics tables

## Directory Structure

```
vc-superpowers/              # Plugin directory
├── commands/                # Slash commands
│   ├── advice.md
│   ├── shoot-the-shit.md
│   ├── research.md
│   ├── stuck.md
│   ├── punch-it-up.md
│   └── vc2-*.md            # 16 secondary command files
├── skills/
│   ├── meta/
│   │   └── using-vc/       # Orientation skill
│   ├── vc/                 # Primary skills
│   │   ├── advice/
│   │   ├── shoot-the-shit/
│   │   ├── research/
│   │   ├── stuck/
│   │   └── punch-it-up/
│   └── secondary/          # 16 secondary skills
│       ├── tam-sam-som-triangulation-SKILL.md
│       ├── unit-economics-and-sensitivity-SKILL.md
│       └── [14 more...]
└── hooks/
    └── session-start.md    # Loads using-vc skill at start

vc-work/                    # Your work directory (gitignored)
├── context.md              # Accumulated inputs
├── session-logs/           # Session logs
│   └── YYYY-MM-DD-HH-MM.md
└── outputs/                # Structured outputs
    └── [topic].md
```

## Contributing

This plugin is designed to be extended. To add a new secondary skill:

1. Create `skills/secondary/[skill-name]-SKILL.md`
2. Follow the pattern in existing skills (Pre-work, Core Questions, Artifacts, MANDATORY Output)
3. Create `commands/vc2-[skill-name].md` that activates the skill
4. Add keyword triggers to relevant primary skills

## License

[Your license here]

## Author

[Your name/contact]

## Acknowledgments

Built for founders navigating the fundraising journey. Inspired by the Superpowers plugin pattern.
