# flatsome-reference-rebuild

A reusable AI skill for rebuilding a WordPress interface inspired by a reference website using **Flatsome Theme** and **UX Builder shortcodes**.

## What this skill does

- Analyzes a reference website or screenshots.
- Breaks the layout into sections.
- Maps each section to Flatsome UX Builder elements.
- Generates Flatsome shortcode drafts.
- Adds custom CSS when needed.
- Produces responsive and QA checklists.

## What this skill does not do

- It does not copy copyrighted website source code.
- It does not copy images, logos, icons, or brand assets.
- It does not hotlink assets from the reference site.
- It does not clone a website pixel-for-pixel.

## Suggested folder path

For Claude Code:

```bash
.claude/skills/flatsome-reference-rebuild/
```

For a general AI skills repository:

```bash
skills/flatsome-reference-rebuild/
```

## Recommended tools

- Playwright MCP: capture screenshots and inspect layout.
- Firecrawl MCP/CLI: map pages and extract content structure.
- WordPress/Flatsome admin access: paste shortcode and verify in UX Builder.

## Example request

```text
Use the flatsome-reference-rebuild skill.
Analyze this reference website: https://example.com
Rebuild a similar homepage layout using Flatsome UX Builder shortcode.
Do not copy images, text, logo, or source code.
Return section mapping, shortcode, custom CSS, and implementation checklist.
```
