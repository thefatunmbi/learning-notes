# CSS Fundamentals

## CSS Syntax

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

## Selectors

### Universal Selector

```css
* {}
```

Selects all elements.

### Type Selector

```css
div {}
```

Selects all elements of a type.

### Class Selector

```css
.alert {}
```

* Starts with `.`
* Reusable on multiple elements

### ID Selector

```css
#title {}
```

* Starts with `#`
* Should be unique on a page

### Grouping Selectors

```css
.read,
.unread {}
```

Apply the same styles to multiple selectors.

### Chaining Selectors

```css
.subsection.header {}
```

Selects elements with both classes.

```css
.subsection#preview {}
```

Selects an element with both the class and ID.

### Descendant Combinator

```css
.ancestor .child {}
```

Selects `.child` only if it is inside `.ancestor`.

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

* Use `auto` to keep image proportions.
* Include `width` and `height` attributes in HTML to prevent layout shifts while images load.

---

## Adding CSS to HTML

### External CSS (Recommended)

```html
<link rel="stylesheet" href="styles.css">
```

* Keeps HTML clean
* Reusable across pages

### Internal CSS

```html
<style>
  p { color: red; }
</style>
```

Used for a single page.

### Inline CSS

```html
<p style="color:red;">Hello</p>
```

Avoid when possible.

---

## Key Takeaways

* `.` = Class
* `#` = ID
* `,` = Group selectors
* No space = Chain selectors
* Space = Descendant combinator
* External CSS is preferred


Here’s a clean, short note you can paste into your `css.md`:

---

# 📦 CSS Box Model

The CSS Box Model describes how every HTML element is structured as a rectangular box made up of:

* **Content** – the actual text or image
* **Padding** – space between content and border
* **Border** – line around the padding/content
* **Margin** – space outside the element (distance from other elements)

```text id="boxmodel1"
margin → border → padding → content → padding → border → margin
```

---

## 📏 Box Sizing

`box-sizing` controls how the total width and height of an element is calculated.

### Default behavior:

```css id="boxmodel2"
box-sizing: content-box;
```

* Width and height apply ONLY to content
* Padding and border are added outside, increasing total size

---

### Recommended setting:

```css id="boxmodel3"
box-sizing: border-box;
```

* Width and height include padding and border
* Makes layout easier and more predictable

---

## 💡 Best Practice

Most developers reset box sizing globally:

```css id="boxmodel4"
* {
  box-sizing: border-box;
}
```

This prevents unexpected layout issues and makes sizing consistent across all elements.

---


