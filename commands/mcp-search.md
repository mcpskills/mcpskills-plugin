---
description: Search for MCP servers in the MCPSkills registry
---

# Search MCP Servers Command

Search the MCPSkills registry for MCP servers matching "$ARGUMENTS".

## Steps

1. First, ensure `mcp-get` CLI is available:
   ```bash
   which mcp-get || npm install -g mcp-get
   ```

2. Search for MCP servers:
   ```bash
   mcp-get search "$ARGUMENTS"
   ```

3. Present the results showing:
   - Server name
   - Description
   - Required configuration (env vars, API keys)
   - Downloads count
   - Install command

4. If the user wants to install any server:
   ```bash
   mcp-get install <server-name>
   ```

## MCP Server Categories

If no search query provided, suggest browsing by category:
- **databases** - PostgreSQL, SQLite, MongoDB connectors
- **apis** - GitHub, Slack, Google Drive integrations
- **search** - Brave Search, web fetching
- **files** - Filesystem access, file operations
- **ai** - Memory, embeddings, AI tool chains
