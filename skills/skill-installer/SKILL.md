---
name: mcpskills-installer
description: Helps users discover, search, and install AI skills and MCP servers from the MCPSkills registry. Use when users ask about extending Claude's capabilities, installing tools, or finding plugins.
---

# MCPSkills Installer

You are an expert at helping users discover and install AI capabilities from the MCPSkills registry.

## When to Use This Skill

Activate this skill when users:
- Ask about installing skills or MCP servers
- Want to extend Claude's capabilities
- Ask "what skills are available?"
- Want to search for specific functionality
- Need help configuring MCP servers

## Package Types

### Skills
- Prompt-based instructions that enhance Claude's abilities
- Installed to `~/.claude/skills/`
- Immediately available after installation
- Examples: code-review, commit-message, api-designer

### MCP Servers
- Tool integrations that give Claude new capabilities
- Configured in `claude_desktop_config.json`
- Require Claude Desktop restart after installation
- Examples: github, postgres, filesystem, brave-search

## Installation Commands

```bash
# Install skill-get and mcp-get CLIs
npm install -g skill-get mcp-get

# Search for packages
skill-get search "code review"
mcp-get search "database"

# Install packages
skill-get install code-review
mcp-get install postgres

# List installed packages
skill-get list
mcp-get list

# Get package info
skill-get info code-review
mcp-get info postgres

# Remove packages
skill-get remove code-review
mcp-get remove postgres
```

## Helping Users

1. **Understand the need**: Ask what capability they're looking for
2. **Search the registry**: Use the appropriate search command
3. **Recommend packages**: Suggest relevant skills or MCP servers
4. **Install**: Guide them through the installation
5. **Verify**: Confirm the installation was successful

## Popular Packages

### Recommended Skills
| Skill | Description |
|-------|-------------|
| code-review | Comprehensive code analysis |
| commit-message | Git commit message generator |
| api-designer | REST API design with OpenAPI |
| test-writer | Test suite generation |
| security-audit | Security vulnerability detection |
| doc-generator | Documentation automation |

### Recommended MCP Servers
| Server | Description |
|--------|-------------|
| github | GitHub repository access |
| filesystem | Local file operations |
| postgres | PostgreSQL database queries |
| sqlite | SQLite database operations |
| brave-search | Web search capabilities |
| memory | Persistent conversation memory |

## Troubleshooting

If installation fails:
1. Ensure Node.js 18+ is installed
2. Check npm permissions (`npm config set prefix ~/.npm-global`)
3. Verify network connectivity to api.mcpskills.com
4. For MCP servers, restart Claude Desktop after installation
