# Web Design Rules and Framework

## 1. Web Design Basics

- **Web design:** Decides how a website looks and feels.
- **Web development:** Implements the design using HTML, CSS and JavaScript.
- Good design builds trust, creates a good first impression and helps users achieve their goals.
- Design choices should match the website's personality.

## 2. Website Personalities

| Personality       | Main characteristics                                                              |
| ----------------- | --------------------------------------------------------------------------------- |
| Serious/Elegant   | Serif fonts, gold or pastel colours, high-quality images and sharp corners.       |
| Minimalist/Simple | Essential content, simple fonts, white backgrounds and few images.                |
| Plain/Neutral     | Neutral colours, small text and structured layouts.                               |
| Bold/Confident    | Large bold headings, bright colours and large colour blocks.                      |
| Calm/Peaceful     | Pastel colours, soft serif headings and matching illustrations.                   |
| Startup/Upbeat    | Sans-serif fonts, light backgrounds, rounded corners and subtle shadows.          |
| Playful/Fun       | Multiple colours, creative fonts, illustrations, rounded elements and animations. |

Choose a personality based on the website's purpose and keep the design elements consistent with it.

## 3. Typography

Typography is the arrangement of text to make it readable and visually appealing.

- **Serif:** Has small strokes at the ends of letters; gives a traditional or classic appearance.
- **Sans-serif:** Has no strokes at the ends; gives a modern and clean appearance.
- Use one or two typefaces per page.
- Choose font sizes from a consistent type scale.
- Normal text can use `16px–32px`; long-form text can use `20px` or more.
- Large headings can use `50px+` with a bold font weight.
- Avoid font weights below `400` for normal text.
- Keep lines under approximately 75 characters.
- Use `line-height: 1.5–2` for normal text.
- Adjust letter spacing when headings look unnatural.
- Avoid justifying text and centering long text blocks.

## 4. Colours

Colours help communicate a website's personality.

- **Red:** Power, passion and excitement.
- **Orange:** Happiness and creativity.
- **Yellow:** Joy and brightness.
- **Green:** Nature, growth and health.
- **Blue:** Trust and professionalism.
- **Purple:** Wealth and wisdom.
- **Pink:** Care and affection.
- **Brown:** Comfort and durability.
- **Black:** Power, elegance and minimalism.

### Colour system

- Start with a **main colour** and a **grey/neutral colour**.
- Add accent colours when necessary.
- **Tints** are lighter versions of colours; **shades** are darker versions.
- Use the main colour to highlight important elements and buttons.
- Use accent colours to make selected sections stand out.
- On dark backgrounds, use lighter text colours.
- Avoid pure black text if it looks too harsh.
- Maintain sufficient contrast: `4.5:1` for normal text and `3:1` for large text.

## 5. Images and Illustrations

Common types include product photos, storytelling photos, illustrations and patterns.

- Choose images that match the website's personality.
- Product photos show products, while storytelling photos communicate a situation or feeling.
- Large images attract more attention, so use them carefully.
- Keep image styles and colours consistent.
- Use illustrations and patterns to add character without distracting from the content.

## 6. Icons

- Use icons when they help explain actions or information.
- Keep their style consistent throughout the website.
- Match icons to the design personality.
- Use simple, thin icons for elegant designs and creative icons for playful designs.
- Avoid unnecessary icons.

## 7. Shadows

- Shadows create depth and help elements stand out.
- Use subtle shadows instead of making every element look raised.
- They are common in startup and playful designs but less common in minimalist and elegant designs.

## 8. Border Radius

The `border-radius` property controls how rounded an element's corners are.

- Rounded corners make designs feel friendlier and more playful.
- Match corner roundness with the overall design style.
- Use it on buttons, cards, images and other suitable elements.

```css
.card {
  border-radius: 8px;
}
```

## 9. Whitespace

Whitespace is the empty space around and between elements.

- It separates content and improves readability.
- Keep related elements close together and unrelated groups farther apart.
- Too little whitespace makes a page cramped; too much can make related elements feel disconnected.
- Larger text and icons usually need more surrounding space.
- Use consistent spacing, such as multiples of `16px`.

## 10. Visual Hierarchy

Visual hierarchy determines which elements users notice first and guides their attention through the page.

- Place important content near the top.
- Larger text and images attract more attention.
- Use whitespace to separate and emphasise elements.
- Position, size, colour, spacing, borders and shadows help establish hierarchy.
- Make the primary action more noticeable than secondary content.

## 11. User Experience (UX)

Good design helps users accomplish their goals easily.

- Make the purpose of the page clear.
- Keep navigation and actions understandable.
- Present information in a logical order.
- Avoid unnecessary distractions.
- Maintain consistent styles and readable text.
- Ensure sufficient colour contrast and easy-to-use controls.

## 12. Components and Layout

- **Page layout:** Arranges the main sections of a webpage.
- **Component layout:** Arranges elements within a section, such as cards, buttons and feature lists.
- Group related content using spacing and alignment.
- Keep component styles consistent.
- Choose layouts that suit the content and website personality.

## 13. Applying the Design Framework

1. Choose the website's personality.
2. Select suitable typography and font sizes.
3. Establish a colour palette.
4. Choose matching images and icons.
5. Decide whether shadows and rounded corners fit the design.
6. Arrange content using whitespace and visual hierarchy.
7. Check readability, contrast and ease of use.
