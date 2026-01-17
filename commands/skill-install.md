---
description: Install an AI skill from the MCPSkills registry
---

# Install Skill Command

Install the skill "$ARGUMENTS" from the MCPSkills registry.

## Steps

1. First, check if `skill-get` CLI is installed by running:
   ```bash
   which skill-get || npm list -g skill-get
   ```

2. If not installed, install it first:
   ```bash
   npm install -g skill-get
   ```

3. Then install the requested skill:
   ```bash
   skill-get install $ARGUMENTS
   ```

4. After installation, inform the user:
   - Where the skill was installed (typically `~/.claude/skills/<skill-name>/`)
   - How to use the skill (it will be automatically available in Claude Code)
   - The skill's description and capabilities

If the user didn't specify a skill name, search for popular skills and recommend some options:
```bash
skill-get search ""
```
