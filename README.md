# Claude Plugins Marketplace

Personal plugin marketplace for Claude Code with specialized agents, commands, and skills.

## Installation

Add this marketplace to Claude Code:

```bash
/plugin marketplace add jrentmeister/claude-plugins
```

## Available Plugins

### Golf Leaderboard (`golf-leaderboard`)
Golf tournament leaderboard development tools with specialized agents for tournament tracking and scoring systems.

**Features:**
- **Agent**: Golf Architect - Specialized in designing scoring systems and real-time leaderboards
- **Command**: `/setup-project` - Scaffold a complete golf leaderboard application
- **Skill**: Golf Scoring Rules - Comprehensive knowledge of tournament formats and scoring

**Install:**
```bash
/plugin install golf-leaderboard@jrentmeister-plugins
```

## Usage

Once the marketplace is added, you can:

1. **Browse available plugins**: `/plugin`
2. **Install a plugin**: `/plugin install plugin-name@jrentmeister-plugins`
3. **List installed plugins**: `/plugin list`
4. **Use plugin commands**: `/command-name` (after installing the plugin)
5. **Access skills**: Skills are automatically available when plugin is installed

## Plugin Structure

Each plugin in this marketplace follows the standard structure:

```
plugins/
└── plugin-name/
    ├── agents/          # Specialized AI agents
    ├── commands/        # Executable slash commands
    └── skills/          # Knowledge packages
```

## Creating Your Own Plugins

To add new plugins to this marketplace:

1. Create a new directory under `plugins/`
2. Add agent definitions (`.md` files) in `plugins/your-plugin/agents/`
3. Add command definitions in `plugins/your-plugin/commands/`
4. Add skill documentation in `plugins/your-plugin/skills/`
5. Update `.claude-plugin/marketplace.json` with your plugin entry
6. Commit and push changes

**Example plugin entry:**
```json
{
  "name": "your-plugin",
  "source": "./plugins/your-plugin",
  "description": "Your plugin description",
  "version": "1.0.0",
  "author": {
    "name": "Your Name",
    "url": "https://github.com/yourusername"
  },
  "license": "MIT",
  "keywords": ["tag1", "tag2"],
  "category": "development",
  "agents": ["./plugins/your-plugin/agents/agent-name.md"],
  "commands": ["./plugins/your-plugin/commands/command-name.md"],
  "skills": ["./plugins/your-plugin/skills/skill-name.md"]
}
```

## License

MIT
