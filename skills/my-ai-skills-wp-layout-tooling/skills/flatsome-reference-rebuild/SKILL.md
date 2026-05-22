---
name: flatsome-reference-rebuild
description: Analyze a page reference, screenshot, or design brief and rebuild an original WordPress layout using Flatsome Theme / UX Builder style shortcodes.
---

# Flatsome Reference Rebuild Skill

## Purpose

Use this skill to create an original WordPress page layout using Flatsome Theme and UX Builder style shortcode structure.

The skill is useful when the user provides:

- A design brief
- Owned screenshots
- Internal approved design references
- A website URL for layout study
- Product/category page requirements
- A landing page structure

The output should help a developer quickly build the page in WordPress/Flatsome.

## Core Principles

1. Use references for layout understanding only.
2. Use the user's own content, images, logo, product data, and brand identity.
3. Do not hotlink assets.
4. Prefer Flatsome native elements before custom code.
5. Keep shortcode nesting clean and editable.
6. Use placeholders clearly where assets/content are missing.
7. Always include desktop, tablet, and mobile notes.
8. Always include implementation and QA checklists.

## Standard Workflow

### 1. Identify Page Type

Classify the page:

- Homepage
- Landing page
- Product category page
- Product detail page
- Service page
- About page
- Blog/news page
- Contact page
- Other

### 2. Break Down The Page

Analyze or design the page section by section:

1. Header/navigation
2. Hero
3. Trust/benefit strip
4. Product/service blocks
5. Feature blocks
6. Process/how-it-works
7. Promotional banner
8. Testimonials/reviews
9. FAQ
10. CTA
11. Footer

For each section, define:

- Purpose
- Layout
- Number of columns
- Content type
- Media usage
- CTA position
- Background style
- Spacing
- Responsive behavior

### 3. Create Design Tokens

Define:

- Primary color
- Secondary color
- Accent color
- Background color
- Text color
- Border color
- Font style category
- Button style
- Border radius
- Shadow style
- Section padding
- Card spacing

### 4. Map To Flatsome Elements

| UI Pattern | Flatsome / UX Builder Element |
|---|---|
| Full-width hero | `[section]` + `[ux_banner]` |
| Text overlay | `[text_box]` |
| CTA button | `[button]` |
| 2-column content | `[row]` + `[col]` |
| Feature grid | `[featured_box]` or `[row]` cards |
| Product grid | `[ux_products]` or WooCommerce shortcode |
| Category grid | `[ux_product_categories]` or custom cards |
| Slider | `[ux_slider]` |
| Testimonials | `[testimonial]` or cards |
| FAQ | `[accordion]` |
| Tabs | `[tabgroup]` |
| Blog/news | `[blog_posts]` |
| Footer CTA | `[section]` + `[button]` |

### 5. Generate UX Builder Structure

Prefer this structure:

```text
[section class="section-name"]
  [row]
    [col span="12"]
      <h2>Placeholder title</h2>
      <p>Placeholder content.</p>
    [/col]
  [/row]
[/section]
```

Hero example:

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

### 6. Add CSS Only When Needed

Use custom CSS for:

- Hover effects
- Responsive spacing
- Gradients
- Badges/ribbons
- Card polish
- Typography tuning

Avoid CSS when Flatsome settings can handle it.

## Output Format

Use this structure:

```markdown
# Flatsome Page Rebuild Plan

## 1. Page Type

## 2. Section Breakdown

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

- Specific enough for implementation
- Structured by page section
- Editable in WordPress/Flatsome
- Clear about placeholders
- Responsive across desktop/tablet/mobile
- Adapted to the user's own brand and assets
