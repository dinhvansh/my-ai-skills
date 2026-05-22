# MCP Setup Notes for Flatsome Reference Rebuild

## Playwright MCP

Use Playwright MCP when you need to inspect a reference website visually.

Suggested install command:

```bash
codex mcp add playwright npx "@playwright/mcp@latest"
```

Use it to:

- Open reference URL
- Capture screenshots
- Inspect page structure
- Test desktop/tablet/mobile
- Validate rebuilt page visually

## Firecrawl

Use Firecrawl when you need sitemap/content structure.

Suggested commands:

```bash
npm install -g firecrawl-cli
firecrawl setup mcp
firecrawl setup skills
```

Use it to:

- Map URLs
- Extract headings
- Extract page content structure
- Understand sitemap

Do not use Firecrawl output to copy text directly. Rewrite all content.

## Suggested Agent Command

```text
Use Playwright MCP to inspect the reference URL at desktop, tablet, and mobile sizes.
Then use the flatsome-reference-rebuild skill to generate a Flatsome UX Builder shortcode draft and custom CSS.
Do not copy source code, text, images, logos, icons, or brand identity.
```
