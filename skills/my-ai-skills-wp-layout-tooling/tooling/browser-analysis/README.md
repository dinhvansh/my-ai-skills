# Browser Analysis Tooling

Tools and prompts for letting an AI assistant inspect a webpage in a browser and convert observations into a page implementation plan.

## Recommended Tools

### 1. Playwright MCP

Use when the assistant needs to open a page, inspect visible structure, capture screenshots, and check responsive behavior.

```bash
codex mcp add playwright npx "@playwright/mcp@latest"
```

Useful for:

- Opening a URL
- Capturing desktop/tablet/mobile screenshots
- Inspecting page structure
- Checking menu, popup, form, and responsive states

### 2. Firecrawl

Use for page inventory, sitemap, headings, metadata, and structured page text.

```bash
npm install -g firecrawl-cli
firecrawl setup mcp
firecrawl setup skills
```

Useful for:

- Mapping site pages
- Reading title/headings/descriptions
- Creating content inventory
- Preparing section-by-section outline

## Suggested Prompt

```md
Use browser analysis tooling.

Open this URL: <URL>

Capture:
1. Desktop layout
2. Mobile layout
3. Header/menu behavior
4. Main sections
5. CTA and product/service blocks

Then produce:
1. Section breakdown
2. WordPress implementation plan
3. Builder structure
4. CSS notes
5. Responsive checklist
6. Asset replacement checklist
```
