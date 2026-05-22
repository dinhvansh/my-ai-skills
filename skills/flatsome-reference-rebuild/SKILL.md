---
name: flatsome-reference-rebuild
description: Rebuild a WordPress page inspired by a reference website using Flatsome Theme and UX Builder shortcodes. Use this skill when the user provides a website URL, screenshots, or a design reference and wants to recreate a similar layout in Flatsome without copying copyrighted assets, source code, logos, images, or text.
---

# Flatsome Reference Rebuild Skill

## Purpose

This skill helps analyze a reference website and rebuild a similar WordPress interface using **Flatsome Theme** and **UX Builder shortcode structure**.

The goal is **reference-based rebuild**, not illegal cloning.

Use this skill to:

- Analyze a reference website layout.
- Break the page into reusable Flatsome sections.
- Convert the layout into Flatsome UX Builder shortcodes.
- Generate custom CSS only when Flatsome native options are not enough.
- Provide responsive rules for desktop, tablet, and mobile.
- Prepare implementation instructions for WordPress/Flatsome.

## Non-Negotiable Rules

Always follow these rules:

1. Do **not** copy copyrighted source code from the reference website.
2. Do **not** copy original images, logos, icons, videos, fonts, or brand identity.
3. Do **not** hotlink assets from the reference website.
4. Do **not** copy text content verbatim from the reference website.
5. Rebuild the layout as an **inspired design** using original content and assets.
6. Prefer Flatsome native elements before custom HTML/CSS.
7. Keep UX Builder shortcode nesting valid.
8. Keep the output practical enough to paste into WordPress/Flatsome.
9. Clearly mark all placeholders that the user must replace.
10. If a layout is legally risky because it is too identical, recommend changing spacing, colors, typography, imagery, icons, and section composition.

## Recommended MCP / Tool Flow

When tools are available, use this workflow:

1. Use browser automation such as Playwright MCP to open the reference URL.
2. Capture screenshots at:
   - Desktop: 1440px width
   - Tablet: 768px width
   - Mobile: 390px width
3. Use crawler/scraper tools such as Firecrawl only to understand page structure, visible text, headings, and sitemap.
4. Never use scraped assets directly in the final build.
5. Analyze visual layout and map it to Flatsome components.
6. Generate shortcodes and CSS.
7. Provide a manual QA checklist for WordPress.

## Flatsome Component Mapping

Map common website sections to Flatsome elements as follows:

| Reference UI Pattern | Flatsome / UX Builder Element |
|---|---|
| Full-width hero | `[section]` + `[ux_banner]` or `[row]` + `[col]` |
| Text overlay on image | `[ux_banner]` + `[text_box]` |
| CTA button | `[button]` |
| 2-column content | `[row]` + two `[col]` elements |
| 3/4 feature grid | `[row]` + `[col]` + `[featured_box]` |
| Product grid | `[ux_products]`, `[products]`, or WooCommerce shortcode |
| Category grid | `[ux_product_categories]` or `[row]` custom category cards |
| Slider / carousel | `[ux_slider]` or `[slider]` |
| Testimonial section | `[testimonial]`, `[row]`, or simple card columns |
| FAQ | `[accordion]` + `[accordion-item]` |
| Tabs | `[tabgroup]` + `[tab]` |
| Logo strip | `[ux_gallery]` or `[row]` image columns |
| Blog/news cards | `[blog_posts]` or custom `[row]` cards |
| Footer CTA | `[section]` + `[row]` + `[button]` |

## Standard Workflow

### Step 1: Identify Page Type

Classify the target page:

- Homepage
- Landing page
- Product category page
- Product detail page
- Service page
- About page
- Blog/news page
- Contact page
- Other

### Step 2: Break Down Page Structure

Analyze the reference page section by section:

1. Header/navigation behavior
2. Hero section
3. Trust/social proof section
4. Product/service blocks
5. Feature/benefit blocks
6. Process/how-it-works section
7. Promotional banners
8. Testimonials/reviews
9. FAQ
10. CTA
11. Footer

For each section, identify:

- Purpose
- Layout
- Number of columns
- Main content type
- Image/video usage
- CTA position
- Background style
- Spacing rhythm
- Responsive behavior

### Step 3: Create Design Tokens

Extract approximate visual direction without copying:

- Primary color
- Secondary color
- Accent color
- Background color
- Text color
- Border color
- Font style category only, not exact copyrighted font unless user owns it
- Button style
- Border radius
- Shadow style
- Section padding
- Card spacing

### Step 4: Convert to Flatsome Structure

Generate UX Builder shortcode using valid Flatsome-style nesting.

Prefer this structure:

```text
[section]
  [row]
    [col]
      content element
    [/col]
  [/row]
[/section]
```

For hero sections:

```text
[section class="hero-section"]
  [ux_banner height="600px" bg="__REPLACE_IMAGE_ID__" bg_overlay="rgba(0,0,0,.35)"]
    [text_box width="60" position_x="10" position_y="50"]
      <h1>Placeholder headline</h1>
      <p>Placeholder subheadline</p>
      [button text="Call to action" link="#"]
    [/text_box]
  [/ux_banner]
[/section]
```

### Step 5: Add Custom CSS Only When Needed

Use custom CSS for:

- Complex card hover effects
- Custom responsive spacing
- Sticky visual behavior
- Special gradients
- Custom badge/ribbon
- Fine-tuned typography

Avoid custom CSS for things Flatsome can already handle natively.

### Step 6: Output Implementation Checklist

Always end with a checklist:

- Replace placeholder images
- Replace placeholder text
- Replace logo/icon assets
- Update product/category IDs
- Test desktop/tablet/mobile
- Check speed/performance
- Check WooCommerce display
- Check legal/copyright safety

## Output Format

Use this exact output structure unless the user asks otherwise:

```markdown
# Flatsome Reference Rebuild Plan

## 1. Page Type

## 2. Reference Layout Breakdown

## 3. Flatsome Section Mapping

## 4. Design Tokens

## 5. UX Builder Shortcode Draft

## 6. Custom CSS

## 7. Responsive Notes

## 8. WordPress Implementation Steps

## 9. Asset Replacement Checklist

## 10. QA Checklist
```

## Quality Bar

A good answer must be:

- Specific enough for a developer to implement.
- Safe from copyright and brand-copying risks.
- Structured by page sections.
- Compatible with Flatsome/UX Builder thinking.
- Practical for WordPress implementation.
- Clear about placeholders and replacement items.

## When User Gives Only a URL

Do not ask unnecessary questions. Make a best-effort analysis using browser/scraper tools if available.

If tools are not available, ask the user to provide screenshots of:

- Full desktop page
- Mobile page
- Important hover/dropdown states
- Product/category sections

## When User Gives Screenshots

Analyze the screenshots visually and produce:

- Section breakdown
- Flatsome mapping
- Shortcode draft
- Custom CSS
- Implementation checklist

## When User Wants Direct Code

Return:

1. Short implementation note
2. Full UX Builder shortcode
3. CSS block
4. Asset replacement list

Do not over-explain.

## Safety Language

When needed, include this reminder:

> This is a reference-based rebuild. Replace all images, text, logos, icons, brand colors, and trademarks with your own assets before publishing.
