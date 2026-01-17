---
description: Search for AI skills in the MCPSkills registry
---

# Search Skills Command

Search the MCPSkills registry for skills matching "$ARGUMENTS".

## Steps

1. First, ensure `skill-get` CLI is available:
   ```bash
   which skill-get || npm install -g skill-get
   ```

2. Search for skills:
   ```bash
   skill-get search "$ARGUMENTS"
   ```

3. Present the results in a formatted table showing:
   - Skill name
   - Description
   - Downloads count
   - Rating (if available)
   - Install command

4. If the user wants to install any skill, use:
   ```bash
   skill-get install <skill-name>
   ```

## Popular Categories

If no search query provided, suggest browsing by category:
- **code-review** - Code analysis and review skills
- **documentation** - Documentation generation
- **testing** - Test writing and coverage
- **security** - Security auditing
- **refactoring** - Code refactoring helpers
