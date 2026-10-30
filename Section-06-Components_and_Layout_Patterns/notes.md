# Components and Layout Patterns

## 1. From Elements to a Complete Webpage

A webpage is created in stages:

**Elements → Components → Layouts → Webpage**

1. Use common elements and components to communicate information.
2. Combine components into layouts using common layout patterns.
3. Assemble different layout areas into a complete webpage.

## 2. Elements

Elements are the basic building blocks of a webpage.

- **Text:** Headings, paragraphs and labels.
- **Buttons:** Allow users to perform actions such as submitting, buying or navigating.
- **Images:** Display products, people, places or visual information.
- **Input elements:** Allow users to enter or select information, such as search fields, dropdowns and quantity controls.
- **Tags:** Small labels used to classify or describe content.

## 3. Components

Components combine elements into reusable interface sections.

1. **Breadcrumbs:** Show the user's current location in a website's hierarchy and provide links to parent pages.
2. **Pagination:** Divides content into multiple pages and provides navigation between them.
3. **Alert and Status Bars:** Display important messages, notifications and status information.
4. **Statistics:** Present numerical information and important figures.
5. **Gallery:** Displays a collection of images or media.
6. **Feature Box:** Highlights a particular feature, service or benefit.
7. **Preview and Profile Cards:** Provide a compact preview of a product, article, person or service.
8. **Accordion:** Organises content into expandable and collapsible sections.
9. **Tabs:** Divide related content into separate views that users can switch between.
10. **Carousel:** Displays multiple items in a sequence, allowing users to move between slides.
11. **Customer Testimonials:** Display customer feedback, reviews and ratings.
12. **Customer Logos:** Display logos of customers or organisations using a service.
13. **Featured-in Logos:** Display publications or media outlets that have featured the company.
14. **Steps:** Explain a process through numbered or ordered stages.
15. **Forms:** Collect information through input fields and selection controls.
16. **Tables:** Organise structured information into rows and columns.
17. **Pricing Tables:** Compare different plans, prices and included features.
18. **Modal Windows:** Display content in an overlay above the current webpage, such as login forms or confirmation messages.

## 4. Building Interactive Components with CSS

### Flex Direction: Column

When `flex-direction` changes from its default row direction to column, the main and cross axes change.

```css
.accordion {
  display: flex;
  gap: 24px;
  flex-direction: column;
}
```

With `flex-direction: column`:

- Main axis becomes vertical.
- Cross axis becomes horizontal.
- `justify-content` aligns items vertically.
- `align-items` aligns items horizontally.
- `gap` creates vertical spacing between items, similar to `margin-bottom`.

### Vertically Centering Carousel Controls

The PDF demonstrates using absolute positioning and transform to vertically center a carousel button.

```css
.carousel {
  position: relative;
}

.btn--left {
  position: absolute;
  top: 50%;
  transform: translate(0, -50%);
}
```

Explanation:

- `position: relative` on the carousel makes it the positioning reference.
- `top: 50%` positions the button at 50% of the parent's height.
- `transform: translate(0, -50%)` moves the button upward by 50% of its own height.
- Together, these properties vertically center the button.

## 5. Section Components

Section components are larger parts of a webpage made by combining smaller elements and components.

### 5.1 Navigation

Navigation helps users move around a website and find important sections.

- Contains links to important pages.
- Can include dropdown menus containing related links.
- Can use overlays to display larger navigation menus.
- Secondary navigation provides additional navigation within a particular section.

### 5.2 Hero Section

The hero section is a prominent section near the top of a webpage.

- Introduces the website, product or service.
- Commonly contains a main heading, supporting text, image or illustration.
- Usually includes a call-to-action button.
- Communicates the main message clearly.

### 5.3 Footer

The footer is the section at the bottom of a webpage.

- Provides additional navigation links.
- Can include company information and contact details.
- May contain social media links and other supporting information.

### 5.4 Call-to-Action (CTA) Section

A CTA section encourages users to perform a particular action.

- Uses clear, action-oriented text.
- Usually contains a prominent button or link.
- Common actions include signing up, starting a trial, requesting a demo or contacting the company.

### 5.5 Feature Row

A feature row presents a product or service feature with supporting information.

- Combines headings, descriptions, images or illustrations.
- Multiple feature rows can be stacked to explain different benefits.
- Text and images can alternate sides.
- Grid or row patterns can be used inside feature rows.

## 6. Layout Patterns

Layout patterns describe how components are arranged on a webpage.

### 6.1 Row of Boxes / Cards

- Places cards next to one another horizontally.
- Useful for displaying related features, steps, benefits or products.
- Cards generally follow a consistent visual structure.

### 6.2 Grid of Boxes / Cards

- Arranges cards into multiple rows and columns.
- Useful for displaying products, services, profiles, features and articles.
- Makes it easier to scan and compare multiple items.
- Grid patterns can also be nested inside larger components.

### 6.3 Z-Pattern

- Guides the user's eyes in a Z-shaped direction.
- The typical reading path moves horizontally across the top, diagonally downward and then horizontally across the next row.
- Useful for pages containing text and visual content arranged to guide attention.

### 6.4 F-Pattern

- Organises content around an F-shaped scanning pattern.
- Users typically scan horizontally across the top, move down the left side and make shorter horizontal scans.
- Useful for text-heavy pages, lists and content containing headings and summaries.

### 6.5 Single-Column Layout

- Places content in one vertical column.
- Users move down the page from one section to another.
- Useful for articles, long-form content and focused reading experiences.

### 6.6 Sidebar Layout

- Places a secondary column beside the main content.
- The sidebar can contain filters, navigation, categories or supporting information.
- The main area displays the primary content.
- Commonly used in product listings, dashboards and information-heavy pages.

### 6.7 Multi-Column / Magazine Layout

- Arranges content into multiple columns.
- Different content items can have different sizes and importance.
- Commonly used for news, editorial and magazine-style websites.

### 6.8 Asymmetry / Experimental Layout

- Uses intentionally uneven or unconventional arrangements.
- Elements may differ in size, position and visual weight.
- Helps create distinctive and creative website designs.
- The layout should still keep content understandable.

## 7. Nesting Layout Patterns

Layout patterns can be used inside other components rather than only at the webpage level.

- A feature row can contain a **grid pattern** to arrange multiple feature items.
- A feature row can contain a **row pattern** to place related items side by side.
- Different sections of the same webpage can use different patterns.
- Choose patterns according to the content and how users should scan it.

## 8. Building a Webpage Using Components and Patterns

1. Identify the information the webpage needs to communicate.
2. Select basic elements such as text, buttons, images and input fields.
3. Combine elements into suitable components.
4. Group components into larger sections such as navigation, hero, feature rows and footer.
5. Select suitable layout patterns for each section.
6. Use nested row or grid patterns when required.
7. Assemble all sections into a complete webpage.
