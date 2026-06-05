# CSS Fundamentals

## What is CSS?

CSS (Cascading Style Sheets) is used to style HTML elements.

Basic syntax:

```css
selector {
  property: value;
}
```

Example:

```css
p {
  color: red;
}
```

---

## Common Selectors

### Universal Selector

Selects every element:

```css
* {
  color: purple;
}
```

### Type Selector

Selects all elements of a type:

```css
div {
  color: white;
}
```

### Class Selector

HTML:

```html
<div class="alert-text"></div>
```

CSS:

```css
.alert-text {
  color: red;
}
```

* Starts with `.`
* Can be used on multiple elements
* Can have multiple classes:

```html
<div class="alert-text severe-alert"></div>
```

### ID Selector

HTML:

```html
<div id="title"></div>
```

CSS:

```css
#title {
  color: red;
}
```

* Starts with `#`
* Should be unique on a page
* Use sparingly

---

## Grouping Selectors

Apply the same styles to multiple selectors:

```css
.read,
.unread {
  color: white;
}
```

---

## Chaining Selectors

Select elements that have multiple classes:

```css
.subsection.header {
  color: red;
}
```

Selects elements with BOTH classes.

---

## Descendant Combinator

Select nested elements:

```css
.ancestor .child {
  color: blue;
}
```

Selects `.child` only if it is inside `.ancestor`.

---

## Common Properties

### Colors

```css
color: red;
background-color: black;
```

### Typography

```css
font-family: Arial, sans-serif;
font-size: 22px;
font-weight: bold;
text-align: center;
```

### Images

Maintain proportions:

```css
img {
  width: 500px;
  height: auto;
}
```

---

## Adding CSS to HTML

### 1. External CSS (Recommended)

HTML:

```html
<link rel="stylesheet" href="styles.css">
```

CSS:

```css
p {
  color: red;
}
```

Advantages:

* Keeps HTML clean
* Reusable across multiple pages

### 2. Internal CSS

```html
<style>
  p {
    color: red;
  }
</style>
```

Used for styles specific to one page.

### 3. Inline CSS

```html
<p style="color:red;">Hello</p>
```

Avoid when possible because it becomes messy and overrides other CSS.

---

## Key Takeaways

* CSS styles HTML.
* Class selector = `.class-name`
* ID selector = `#id-name`
* Group selectors with commas.
* Chain selectors without spaces.
* Descendant combinator uses a space.
* External CSS is the preferred method.
* Most-used properties:

  * color
  * background-color
  * font-family
  * font-size
  * font-weight
  * text-align
  * width
  * height

```
```
