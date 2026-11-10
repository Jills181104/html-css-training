## Responsive Design – Breakpoints and Media Queries

### 1. Selecting Breakpoints

Breakpoints are screen-width points where the website layout changes to fit different screen sizes.

**Strategies for selecting breakpoints:**

- **Bad:** Choosing breakpoints based on popular device sizes (specific phones, tablets, laptops).
- **Good:** Choosing breakpoints based on screen-width ranges.
- **Best:** Choosing breakpoints wherever the design starts breaking or looking incorrect.

The main idea is to make the layout responsive based on the content, not specific devices.

### 2. How Media Queries Work (max-width)

Media queries apply CSS styles only when a particular condition is satisfied.

**Syntax:**

```css
@media (max-width: 600px) {
  /* CSS rules */
}
```

- max-width: 600px means the CSS applies when the viewport width is 600px or less.
- max-width: 1200px means the CSS applies when the viewport width is 1200px or less.
