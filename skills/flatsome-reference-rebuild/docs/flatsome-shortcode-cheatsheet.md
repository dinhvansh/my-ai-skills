# Flatsome Shortcode Cheatsheet

## Basic Section

```text
[section]
  [row]
    [col span="12"]
      <h2>Title</h2>
      <p>Content</p>
    [/col]
  [/row]
[/section]
```

## Two Columns

```text
[row]
  [col span="6" span__sm="12"]
    <h2>Left column</h2>
  [/col]
  [col span="6" span__sm="12"]
    <p>Right column</p>
  [/col]
[/row]
```

## Hero Banner

```text
[ux_banner height="600px" bg="__IMAGE_ID__" bg_overlay="rgba(0,0,0,.35)"]
  [text_box width="60" position_x="10" position_y="50"]
    <h1>Hero headline</h1>
    <p>Hero subheadline</p>
    [button text="Start Now" link="#"]
  [/text_box]
[/ux_banner]
```

## Feature Box

```text
[featured_box img="__ICON_ID__" img_width="48"]
  <h4>Feature title</h4>
  <p>Feature description.</p>
[/featured_box]
```

## Products

```text
[ux_products columns="4" columns__sm="2" products="8" orderby="date"]
```

## Blog Posts

```text
[blog_posts columns="3" posts="3" image_height="56%"]
```

## Accordion

```text
[accordion]
  [accordion-item title="Question one"]
    Answer content.
  [/accordion-item]
[/accordion]
```
