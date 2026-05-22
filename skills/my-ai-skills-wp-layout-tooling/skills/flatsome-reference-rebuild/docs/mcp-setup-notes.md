# MCP Setup Notes

## Playwright MCP

Use Playwright MCP for browser viewing, screenshots, DOM/accessibility snapshot, and responsive checks.

```bash
codex mcp add playwright npx "@playwright/mcp@latest"
```

Suggested viewport checks:

- Desktop: 1440px
- Tablet: 768px
- Mobile: 390px

## Firecrawl

Use Firecrawl for sitemap, page inventory, headings, and structured text.

```bash
npm install -g firecrawl-cli
firecrawl setup mcp
firecrawl setup skills
```

## Suggested Workflow

```txt
URL or screenshot
↓
Browser screenshot and layout observation
↓
Content/page structure inventory
↓
Section mapping
↓
Flatsome shortcode draft
↓
CSS notes
↓
Responsive QA
```
