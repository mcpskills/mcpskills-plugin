---
description: Browse the MCPSkills registry for skills and MCP servers
---

# Browse MCPSkills Registry

Browse the MCPSkills registry to discover skills and MCP servers.

## Overview

MCPSkills is the unified registry for AI agent capabilities - both skills (prompts/instructions) and MCP servers (tool integrations).

## Steps

1. Ensure the CLI tools are installed:
   ```bash
   npm list -g skill-get mcp-get || npm install -g skill-get mcp-get
   ```

2. List available skills:
   ```bash
   skill-get search ""
   ```

3. List available MCP servers:
   ```bash
   mcp-get search ""
   ```

4. Show currently installed items:
   ```bash
   skill-get list
   mcp-get list
   ```

## Quick Links

- **Web Marketplace**: https://mcpskills.dev
- **Documentation**: https://mcpskills.dev/docs
- **API**: https://api.mcpskills.dev/api/v1

## Featured Packages

### Top Skills
- `code-review` - Comprehensive code review with security analysis
- `commit-message` - Generate conventional commit messages
- `api-designer` - Design RESTful APIs with OpenAPI specs
- `test-writer` - Generate comprehensive test suites
- `doc-generator` - Auto-generate documentation

### Top MCP Servers
- `github` - Full GitHub API access
- `filesystem` - Secure file system operations
- `postgres` - PostgreSQL database queries
- `brave-search` - Web search capabilities
- `memory` - Persistent memory for conversations

## Usage

After browsing, install with:
```bash
skill-get install <skill-name>
mcp-get install <server-name>
```
