## 1. What is CSS?

**CSS (Cascading Style Sheets)** controls how HTML content looks on a webpage. It is used for colors, fonts, spacing, layout, borders, and more.

## 2. CSS Rule: How We Style Elements

```css
h1 {
  color: blue;
  text-align: center;
  font-size: 20px;
}
```

- **Selector** — `h1`; chooses which HTML element to style.
- **Declaration block** — everything inside `{ }`.
- **Declaration** — one instruction, such as `color: blue;`.
- **Property** — what you want to change, such as `color`.
- **Value** — the setting, such as `blue`.

## 3. The RGB Color Model

RGB stands for **Red, Green, Blue**. A color is created by mixing different amounts of these three light colors. Each channel usually ranges from **0 to 255**

- `rgb(red, green, blue)` sets a color with values from 0 to 255.
- `rgba(red, green, blue, alpha)` also sets transparency.
- **Alpha** ranges from `0` (fully transparent) to `1` (fully opaque).

### Hexadecimal notation

Hex colors start with `#` and use digits `0–9` and letters `a–f`.

```css
color: #00ffff;
```

The six digits represent red, green, and blue in pairs: `#RRGGBB`.

A three-digit shorthand works when each pair repeats:

```css
color: #0ff; /* same as #00ffff */
```

> When all three RGB channels have the same value, the color is grey.

## 1. Conflicting Selectors and Declarations

More than one CSS rule can target the same element. If they set the same property to different values, CSS decides which value wins using **the cascade**.

```html
<p id="author-text" class="author">Posted by Laura</p>
```

```css
.author {
  font-size: 18px;
}
#author-text {
  font-size: 20px;
}
p {
  font-size: 22px;
}
```

All three rules match, but the ID selector wins for `font-size`, so the text is `20px`.

### Basic priority order

From lower to higher priority:

1. Universal selector: `*`
2. Element selector: `p`, `h1`
3. Class / pseudo-class: `.author`, `:hover`
4. ID selector: `#author-text`
5. Inline style: `style="..."`
6. `!important` declarations can override normal declarations.

If competing declarations have the same priority, the one later in the stylesheet usually wins.

## 2. Inheritance

Some CSS properties pass from a parent element to its children.

```css
body {
  color: #444;
  font-family: sans-serif;
  font-size: 16px;
}
```

Text inside the body generally inherits these text-related properties unless another rule overrides them.

- Common inherited properties: `color`, `font-family`, `font-size`, `line-height`.
- Properties such as `border`, `margin`, and `padding` are **not inherited** by default.
- A child’s own CSS rule can override an inherited value.

## 3. The CSS Box Model

Every element is treated as a box made up of:

1. **Content** — text, images, or other content.
2. **Padding** — space around the content, inside the border.
3. **Border** — line surrounding the padding and content.
4. **Margin** — space outside the border, between elements.

### Width and height calculation

With the default `box-sizing: content-box`:

```text
Total width = content width + left/right padding + left/right border
Total height = content height + top/bottom padding + top/bottom border
```

> Margins add space outside the box and are not included in these totals.

## 4. Block, Inline and Inline-Block

- **Block:** Starts on a new line; usually takes full available width. `div`, `p`, `h1`.
- **Inline:** Stays in the text line; uses only needed space. `span`, `a`, `strong`.
- **Inline-block:** Stays inline but allows `width` and `height`.

```css
div {
  display: block;
}
span {
  display: inline;
}
button {
  display: inline-block;
  width: 120px;
}
```

## 5. Normal Flow vs. Absolute Positioning

- **Normal flow:** Elements appear in HTML order; block elements stack vertically.
- `position: static` is the default.
- `position: relative` keeps the element in flow and allows offsets.
- **Absolute:** Removes the element from normal flow and may overlap others. It is positioned relative to its nearest positioned ancestor.

```css
.container {
  position: relative;
}
.box {
  position: absolute;
  top: 100px;
  left: 200px;
}
```

`top`, `bottom`, `left`, and `right` set the offset.

## 6. Margin Collapsing

Margin collapsing occurs when the vertical margins of two block elements combine into a single margin instead of being added together.

Example:

```css
.box1 {
  margin-bottom: 30px;
}

.box2 {
  margin-top: 20px;
}
```

The gap between the elements is 30px, not 50px, because the larger positive margin wins.

> Default size of font is 16px.

> in anchor tag margin does not work because it is inline element and in inline element margin top and botton does not work.

> pseudo class are written with one colon and pseudo elements with two colons
