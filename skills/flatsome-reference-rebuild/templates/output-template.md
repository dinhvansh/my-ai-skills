# Flatsome Reference Rebuild Plan

## 1. Page Type

- Type:
- Goal:
- Main conversion action:

## 2. Reference Layout Breakdown

| Section | Purpose | Layout | Key Elements | Responsive Behavior |
|---|---|---|---|---|
| Header |  |  |  |  |
| Hero |  |  |  |  |
| Section 1 |  |  |  |  |
| Section 2 |  |  |  |  |
| Footer |  |  |  |  |

## 3. Flatsome Section Mapping

| Reference Section | Flatsome Elements | Notes |
|---|---|---|
| Header | Theme Options / Header Builder |  |
| Hero | `[section]` + `[ux_banner]` + `[text_box]` |  |
| Feature grid | `[row]` + `[col]` + `[featured_box]` |  |
| Product grid | `[ux_products]` |  |
| FAQ | `[accordion]` |  |

## 4. Design Tokens

```css
:root {
  --brand-primary: #REPLACE;
  --brand-secondary: #REPLACE;
  --brand-accent: #REPLACE;
  --brand-bg: #REPLACE;
  --brand-text: #REPLACE;
  --brand-muted: #REPLACE;
  --radius-card: 16px;
  --shadow-card: 0 12px 30px rgba(0,0,0,.08);
}
```

## 5. UX Builder Shortcode Draft

```text
[section class="rebuild-section"]
  [row]
    [col span="12"]
      <h2>Placeholder title</h2>
      <p>Placeholder content.</p>
    [/col]
  [/row]
[/section]
```

## 6. Custom CSS

```css
/* Add to Flatsome > Advanced > Custom CSS or child theme */
```

## 7. Responsive Notes

- Desktop:
- Tablet:
- Mobile:

## 8. WordPress Implementation Steps

1. Create a new page in WordPress.
2. Open with UX Builder.
3. Add section structure or paste shortcode where supported.
4. Replace placeholder images with original assets.
5. Replace placeholder text with original business content.
6. Update WooCommerce product/category IDs.
7. Apply custom CSS.
8. Test responsive layout.

## 9. Asset Replacement Checklist

- [ ] Logo replaced
- [ ] Images replaced
- [ ] Icons replaced
- [ ] Text rewritten
- [ ] Brand colors changed
- [ ] Product IDs updated
- [ ] Links updated
- [ ] Tracking scripts reviewed

## 10. QA Checklist

- [ ] Desktop layout checked
- [ ] Tablet layout checked
- [ ] Mobile layout checked
- [ ] Header menu checked
- [ ] CTA buttons checked
- [ ] Product grid checked
- [ ] Forms checked
- [ ] Page speed checked
- [ ] No hotlinked assets
- [ ] No copied content
