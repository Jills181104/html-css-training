# CSS Layouts

## 1. What Is Layout?

A **layout** is how text, images, and other elements are arranged on a webpage.

- **Page layout:** Arrangement of major sections across the page.
- **Component layout:** Arrangement of elements inside one section.

## 2. Three Ways to Build Layouts

- **Float:** Older method, mainly for wrapping text around elements.
- **Flexbox:** One-dimensional layouts (row or column), alignment, and spacing.
- **CSS Grid:** Two-dimensional layouts using rows and columns.

## 3. Normal Flow, Absolute Positioning and Floats

- **Normal flow:** Elements follow their order in the HTML.
- **Absolute positioning:** Removes an element from normal flow; it may overlap other content.
- **Float:** Moves an element left or right and lets text wrap around it.

## 4. `box-sizing: border-box`

By default, width and height apply to the content only, with padding and borders added outside. With `border-box`, declared width and height include content, padding, and border. Margin remains outside.

```css
* {
  box-sizing: border-box;
}
```

## 5. Flexbox

Flexbox is for **one-dimensional layouts**. The parent is the flex container; its direct children are flex items.

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 12px;
  flex-wrap: wrap;
}
```

- `flex-direction`: row or column (also reverse versions).
- `justify-content`: aligns items on the **main axis**.
- `align-items`: aligns items on the **cross axis**.
- `gap`: space between items; `flex-wrap` allows items to wrap.
- Item properties: `align-self`, `flex-grow`, `flex-shrink`, `flex-basis`, `order`.
- `align-content` aligns multiple flex lines when wrapping occurs.

## 6. CSS Grid

Grid is for **two-dimensional layouts** using rows and columns.

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
}
```

- **Container:** Element with `display: grid`; direct children are **grid items**.
- **Tracks:** Rows or columns; **grid lines** mark their boundaries.
- **Grid cell:** One row-column space; **gaps/gutters** are spaces between tracks.
- `grid-template-columns/rows`: define tracks.
- `gap`, `row-gap`, `column-gap`: set spacing.
- `justify-items` / `align-items`: align items inside cells.
- `justify-content` / `align-content`: align the whole grid when extra space exists.
- `grid-column` / `grid-row`: place an item across tracks; `span` covers multiple tracks.
- `justify-self` / `align-self`: align one item.

> Collapsing elements - Collapsing elements (collapsed parent) in CSS happens when all the children inside a parent are floated. Floated elements are removed from the normal document flow, so the parent may calculate its height as 0px.
> Fix it using display: flow-root;
