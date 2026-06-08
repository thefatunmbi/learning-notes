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
*           /* Universal */
div         /* Type */
.class      /* Class */
#id         /* ID */
.a, .b      /* Grouping */
.a.b        /* Chaining */
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

* `auto` keeps image proportions.
* Include `width` and `height` attributes in HTML to prevent layout shifts.

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

Every element consists of:

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

Width/height apply only to content.

### Recommended

```css
box-sizing: border-box;
```

Width/height include padding and border.

Global reset:

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

Space between boxes = `50px`, not `70px`.

**Rule:** The larger vertical margin wins.
