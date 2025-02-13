# CSS Display Methods

## Introduction
CSS provides various display methods that define how elements are rendered on a web page. The most common ones include `block`, `inline`, `flex`, `inline-flex`, and `grid`.

## Display Types

### 1. Block
- Elements take up the full width of their parent container.
- Starts on a new line.
- Examples: `<div>`, `<p>`, `<h1>`

```css
.block-element {
  display: block;
  width: 100%;
  background-color: lightgray;
}
```

### 2. Inline
- Elements only take up as much width as their content.
- Does not start on a new line.
- Examples: `<span>`, `<a>`

```css
.inline-element {
  display: inline;
  color: blue;
}
```

### 3. Inline-Flex
- Behaves like an inline element but retains flexbox properties.
- Allows child elements to be flex items while staying inline.

```css
.inline-flex-container {
  display: inline-flex;
  gap: 10px;
}
```

### 4. Flexbox
- A layout model that arranges elements along a flexible row or column.
- Provides easy alignment and spacing.

```css
.flex-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

### 5. Grid
- Defines a two-dimensional layout system (rows and columns).
- Offers precise placement and alignment.

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
```

## Justify vs Align Properties

### Justify-Content (Main Axis)
Controls alignment along the main axis (horizontal in `row`, vertical in `column`).

```css
.flex-container {
  display: flex;
  justify-content: space-between;
}
```

### Align-Items (Cross Axis)
Aligns items along the cross axis of a flex container.

```css
.flex-container {
  display: flex;
  align-items: center;
}
```

### Align-Content
Controls the spacing between rows in a flex or grid container when there’s extra space.

```css
.flex-container {
  display: flex;
  flex-wrap: wrap;
  align-content: space-between;
}
```

## Conclusion
CSS display methods provide powerful layout control, whether using `block`, `inline`, `flex`, or `grid`. Understanding how to use `justify-content`, `align-items`, and `align-content` helps create well-structured designs.
