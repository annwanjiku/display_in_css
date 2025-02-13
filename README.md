# CSS Display Methods

## Introduction
CSS `display` property controls how elements are rendered in the web-page. Below are the key display methods:

### 1. Block
- Elements take up the full width of their container.
- Starts on a new line.
- Example:
  ```css
  div {
    display: block;
  }
  ```

### 2. Inline
- Elements take up only as much width as needed.
- Does not start on a new line.
- Example:
  ```css
  span {
    display: inline;
  }
  ```

### 3. Inline-Block
- Similar to inline but allows setting width and height.
- However, if the content does not fit —especially when working with text, it behaves like block.
- Example:
  ```css
  button {
    display: inline-block;
    width: 100px;
    height: 50px;
  }
  ```

### 4. Flex (Flexbox)
- A layout model for distributing space among items in a container.
- Use `display: flex;` to activate it.
- Example:
  ```css
  .container {
    display: flex;
  }
  ```

### 5. Inline-Flex
- Behaves like `inline-block` but with flex properties.
- Example:
  ```css
  .container {
    display: inline-flex;
  }
  ```

### 6. Grid
- A two-dimensional layout system.
- Use `display: grid;` to enable it.
- Example:
  ```css
  .grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
  ```

## Alignment Properties

### Justify-Content (Main Axis)
- Controls horizontal alignment in flexbox and grid.
- Example:
  ```css
  .container {
    display: flex;
    justify-content: center; /* Aligns items in the center */
  }
  ```

### Align-Items (Cross Axis)
- Aligns items along the perpendicular axis in flexbox and grid.
- Example:
  ```css
  .container {
    display: flex;
    align-items: center; /* Aligns items to the middle */
  }
  ```

### Align-Content
- Aligns multiple rows in a flex or grid container.
- Example:
  ```css
  .container {
    display: flex;
    flex-wrap: wrap;
    align-content: space-between;
  }
  ```

## Conclusion
Understanding these display properties helps in building responsive and efficient layouts. Use `flexbox` for one-dimensional layouts and `grid` for two-dimensional layouts.
[Examples](https://annwanjiku.github.io/displayIncss/)

