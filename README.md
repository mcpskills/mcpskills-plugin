# MCPSkills Plugin for Claude Code

The official Claude Code plugin for the MCPSkills registry - the Homebrew for AI agents.

## Features

- **Slash Commands**: Quick access to install and search packages
- **Agent Skills**: Intelligent package discovery and installation guidance
- **Registry Integration**: Direct access to the MCPSkills marketplace

## Installation

### From Claude Code Plugin Marketplace

1. Open Claude Code
2. Go to Plugin Manager
3. Search for "mcpskills"
4. Click Install

### Manual Installation

```bash
# Clone the plugin
git clone https://github.com/mcpskills/mcpskills-plugin.git ~/.claude/plugins/mcpskills

# Or test locally
claude --plugin-dir ./mcpskills-plugin
```

## Commands

| Command | Description |
|---------|-------------|
| `/mcpskills:skill-install <name>` | Install a skill from the registry |
| `/mcpskills:skill-search <query>` | Search for skills |
| `/mcpskills:mcp-install <name>` | Install an MCP server |
| `/mcpskills:mcp-search <query>` | Search for MCP servers |
| `/mcpskills:browse` | Browse the full registry |

## Usage Examples

### Install a Skill

```
/mcpskills:skill-install code-review
```

### Search for MCP Servers

```
/mcpskills:mcp-search database
```

### Browse the Registry

```
/mcpskills:browse
```

## Prerequisites

The plugin will automatically install the CLI tools if needed:

- `skill-get` - CLI for managing AI skills
- `mcp-get` - CLI for managing MCP servers

You can also install them manually:

```bash
npm install -g skill-get mcp-get
```

## Links

- **Web Marketplace**: https://mcpskills.dev
- **API Documentation**: https://api.mcpskills.dev/docs
- **GitHub**: https://github.com/mcpskills

## Support

- [Report Issues](https://github.com/mcpskills/mcpskills-plugin/issues)
- [Discord Community](https://discord.gg/mcpskills)
- [Documentation](https://mcpskills.dev/docs)

## License

MIT License - see [LICENSE](LICENSE) for details.
