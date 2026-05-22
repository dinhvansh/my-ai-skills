# Flatsome Shortcode Cheatsheet

## Basic Section

```text
[section]
  [row]
    [col span="12"]
      Content
    [/col]
  [/row]
[/section]
```

## Two Columns

```text
[row]
  [col span="6" span__sm="12"]
    Left content
  [/col]
  [col span="6" span__sm="12"]
    Right content
  [/col]
[/row]
```

## Hero Banner

```text
[ux_banner height="600px" bg="__IMAGE_ID__"]
  [text_box width="60" position_x="10" position_y="50"]
    <h1>Headline</h1>
    <p>Subheadline</p>
    [button text="CTA" link="#"]
  [/text_box]
[/ux_banner]
```

## Product Grid

```text
[ux_products columns="4" columns__sm="2" products="8" orderby="date"]
```

## Category Grid

```text
[ux_product_categories number="8" columns="4" columns__sm="2"]
```

## FAQ

```text
[accordion]
  [accordion-item title="Question 1"]
    Answer 1
  [/accordion-item]
  [accordion-item title="Question 2"]
    Answer 2
  [/accordion-item]
[/accordion]
```
