# Aikido Security — Claude Code Plugin

Brings [Aikido Security](https://aikido.dev) scanning directly into Claude Code. Detects SAST vulnerabilities, exposed secrets, and IaC misconfigurations in code you write or modify, and guides Claude to fix them before they ship.

## Skills

| Skill | Command | Description |
|---|---|---|
| Scan | `/aikido:scan` | Scans modified or new files for security issues, applies fixes, and re-scans until clean |
| Setup | `/aikido:setup` | Verifies the plugin is configured and walks through API key setup if not |

## Requirements

- Node.js 18+
- An Aikido API key — get one at [app.aikido.dev](https://app.aikido.dev) → Settings → Integrations → IDE Plugins

## Installation

Install the plugin from the Claude Code marketplace, then set your API key:

```bash
export AIKIDO_API_KEY="your-key-here"
```

To persist it, add the line above to your shell profile (`~/.zshrc`, `~/.bashrc`, etc.) and restart Claude Code.

Run `/aikido:setup` to verify everything is working.

## More information

- [Aikido MCP documentation](https://help.aikido.dev/mcp/anthropic-claude-code-mcp)
- [Aikido Security](https://aikido.dev)
