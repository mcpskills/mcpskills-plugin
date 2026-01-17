---
description: Install an MCP server from the MCPSkills registry and configure it for Claude Desktop
---

# Install MCP Server Command

Install the MCP server "$ARGUMENTS" from the MCPSkills registry.

## Steps

1. First, check if `mcp-get` CLI is installed:
   ```bash
   which mcp-get || npm list -g mcp-get
   ```

2. If not installed, install it first:
   ```bash
   npm install -g mcp-get
   ```

3. Then install the requested MCP server:
   ```bash
   mcp-get install $ARGUMENTS
   ```

4. The CLI will automatically:
   - Download and install the MCP server
   - Update `claude_desktop_config.json` with the server configuration
   - Prompt for any required environment variables (API keys, tokens, etc.)

5. After installation, inform the user:
   - The server has been configured for Claude Desktop
   - They need to **restart Claude Desktop** for the server to be available
   - What capabilities the MCP server provides

## Common MCP Servers

If no server name provided, suggest popular options:
- **github** - GitHub repository access
- **filesystem** - Local file system access
- **postgres** - PostgreSQL database queries
- **brave-search** - Web search via Brave
- **sqlite** - SQLite database operations
- **slack** - Slack workspace integration
