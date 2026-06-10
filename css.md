# CSS Fundamentals

## CSS Syntax

```css
selector {
  property: value;
}
```

---

## Selectors

```css
*              /* Universal */
div            /* Type */
.class         /* Class */
#id            /* ID */
.a, .b         /* Grouping */
.a.b           /* Chaining */
.parent .child /* Descendant */
```

### Remember

* `.` = Class
* `#` = ID
* `,` = Group selectors (OR)
* No space = Chain selectors (AND)
* Space = Descendant combinator

---

## Common Properties

```css
color
background-color
font-family
font-size
font-weight
text-align
width
height
```

---

## Images

```css
img {
  width: 500px;
  height: auto;
}
```

* `auto` keeps image proportions
* Always set `width` and `height` in HTML to prevent layout shift

---

## Adding CSS

### External (Recommended)

```html
<link rel="stylesheet" href="styles.css">
```

### Internal

```html
<style></style>
```

### Inline

```html
style=""
```

---

# Box Model

Every element is a rectangular box made of:

```text
Margin → Border → Padding → Content
```

* Content = actual content
* Padding = space inside border
* Border = outline around element
* Margin = space outside element

---

## Box Sizing

### Default

```css
box-sizing: content-box;
```

Width and height apply only to content.

### Recommended

```css
box-sizing: border-box;
```

Width and height include padding and border.

### Global Reset

```css
* {
  box-sizing: border-box;
}
```

---

## Margin Collapsing

Vertical margins do not add together.

```css
.box1 {
  margin-bottom: 50px;
}

.box2 {
  margin-top: 20px;
}
```

Space between boxes = **50px**, not 70px.

> The larger vertical margin wins.

---

# Display: Block, Inline, Inline-Block

## Block

* Takes full width
* Starts on a new line
* Width, height, margin, padding work normally

---

## Inline

* Takes only needed space
* Stays on same line
* Cannot set width/height properly

---

## Inline-Block

* Stays on same line like inline
* Supports width and height like block
* Useful for buttons and nav items

---

## Key Difference

* **Block** → new line, full box
* **Inline** → same line, text flow
* **Inline-block** → inline + controllable box

---

## Why Inline-Block is Useful

Inline elements like `<a>` behave like text, so padding doesn’t create a good clickable area.

By using `inline-block`, you can improve usability:

```css
a {
  display: inline-block;
  padding: 10px 15px;
}
```

Now the entire padded area becomes clickable, making it better for buttons and navigation links.

---

