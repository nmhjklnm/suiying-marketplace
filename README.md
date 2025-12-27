# Suiying (随影)

My personal Claude Code plugin - a self-hosted collection of preferred configs, workflows, and development practices.

## Structure

```
suiying-plugin/
├── .claude-plugin/
│   └── plugin.json      # Plugin manifest
├── commands/            # Custom slash commands
├── skills/              # Auto-activating knowledge
├── agents/              # Specialized subagents
├── hooks/               # Event-driven automation
└── scripts/             # Helper utilities
```

## Installation

```bash
# Option 1: Use directly with Claude Code
claude --plugin-dir /path/to/suiying-plugin

# Option 2: Symlink to global plugins
ln -s /path/to/suiying-plugin ~/.claude/plugins/suiying
```

## Usage

After installation, all commands, skills, and agents become available in Claude Code automatically.

## Adding New Components

### Add a Command
Create `commands/your-command.md`:
```markdown
---
name: your-command
description: What this command does
---

Instructions for Claude...
```

### Add a Skill
Create `skills/your-skill/SKILL.md`:
```markdown
---
name: Your Skill
description: When to activate this skill
---

Knowledge and instructions...
```

### Add an Agent
Create `agents/your-agent.md`:
```markdown
---
description: Agent's role
---

Agent system prompt...
```

## License

MIT
