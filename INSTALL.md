# Installation Guide

## Prerequisites

- [Claude Code](https://docs.claude.com/en/docs/claude-code) installed and configured
- Git (for cloning the repository)

## Method 1: Git Clone (Recommended)

This method allows you to easily pull updates.

### Step 1: Clone the Repository

```bash
# Navigate to your Claude Code plugins directory
cd ~/.claude/plugins

# Clone this repository
git clone https://github.com/[your-username]/vc-superpowers.git
```

### Step 2: Create vc-work Directory

You can either create it manually or let Claude create it on first use:

**Option A: Create manually**
```bash
mkdir -p ~/vc-work/session-logs ~/vc-work/outputs
touch ~/vc-work/context.md
```

**Option B: Let Claude create it**
On your first run of any `/vc:` command, Claude will create the directory structure for you.

### Step 3: Restart Claude Code

Restart Claude Code to load the new plugin.

### Step 4: Verify Installation

Run this command in Claude Code:

```
/help
```

You should see `/vc:advice`, `/vc:shoot-the-shit`, etc. in the list of available commands.

### Step 5: Test the Plugin

Run your first command:

```
/vc:advice
```

Claude should:
1. Read `~/vc-work/context.md`
2. Ask you to paste a question
3. Guide you through the advisory flow
4. Create an output file in `~/vc-work/outputs/`

## Method 2: Manual Download

If you don't want to use git:

### Step 1: Download

Download the repository as a ZIP file from GitHub and extract it.

### Step 2: Move to Plugins Directory

```bash
mv vc-superpowers ~/.claude/plugins/
```

### Step 3-5: Same as Method 1

Follow steps 2-5 from Method 1 above.

## Installation on Multiple Machines

To use this plugin on multiple computers:

### Method A: Git (Recommended)

On each machine:
```bash
cd ~/.claude/plugins
git clone https://github.com/[your-username]/vc-superpowers.git
```

Your `~/vc-work/` data is separate on each machine (gitignored), but you can:
- Sync `vc-work/` via Dropbox/Google Drive
- Copy `context.md` manually between machines
- Use git to manage your `vc-work/` directory separately

### Method B: Shared vc-work Directory

If you want to share your vc-work data across machines:

```bash
# On Machine 1: Move vc-work to Dropbox
mv ~/vc-work ~/Dropbox/vc-work
ln -s ~/Dropbox/vc-work ~/vc-work

# On Machine 2: Symlink to Dropbox
ln -s ~/Dropbox/vc-work ~/vc-work
```

Now all machines share the same context.md and outputs.

## Updating the Plugin

If you installed via git clone:

```bash
cd ~/.claude/plugins/vc-superpowers
git pull origin main
```

Restart Claude Code.

## Customizing vc-work Location

By default, the plugin uses `~/vc-work/`. To use a different location:

1. Edit all SKILL.md files and replace `vc-work/` with your path
2. Or, create a symlink:

```bash
ln -s /path/to/your/vc-work ~/vc-work
```

## Troubleshooting

### Plugin Not Showing Up

- Verify it's in `~/.claude/plugins/vc-superpowers/`
- Check that `commands/advice.md` exists
- Restart Claude Code

### "File not found" errors

- Verify `~/vc-work/` exists
- Check permissions: `ls -la ~/vc-work`
- Create manually if needed (see Step 2 above)

### Skills Not Auto-Loading

- This is expected on first use if you haven't added content to `context.md` yet
- Try pasting text with keywords like "TAM" or "unit economics"
- Check that secondary skills exist: `ls ~/.claude/plugins/vc-superpowers/skills/secondary/`

### Commands Not Working

- Run `/help` to see available commands
- Verify naming: commands are `/vc:advice` (with colon), not `/vc-advice`
- Check command files have proper frontmatter (description field)

## Uninstalling

```bash
rm -rf ~/.claude/plugins/vc-superpowers

# Optionally remove your work directory
# (CAUTION: This deletes all your vc-work data)
# rm -rf ~/vc-work
```

## Next Steps

- Read [README.md](./README.md) for usage examples
- Try `/vc:advice` with a real question
- Explore `/vc2:` commands for specific checklists
