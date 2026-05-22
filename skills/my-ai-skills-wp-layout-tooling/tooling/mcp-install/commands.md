# MCP Install Commands

## Playwright MCP

```bash
codex mcp add playwright npx "@playwright/mcp@latest"
```

## Firecrawl CLI + MCP

```bash
npm install -g firecrawl-cli
firecrawl setup mcp
firecrawl setup skills
```

## Suggested Check

After installing, restart your AI coding tool and ask:

```md
Can you list available MCP tools and confirm Playwright/Firecrawl are available?
```

## Common Troubleshooting

- Restart terminal/IDE after install.
- Make sure Node.js and npm are installed.
- Run commands from the project root when possible.
- If using Codex/Claude/Cursor, check each tool's MCP config file.
