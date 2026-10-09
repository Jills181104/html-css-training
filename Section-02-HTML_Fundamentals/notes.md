# Section 02 — HTML Fundamentals

## 1. Introduction to HTML

**HTML (HyperText Markup Language)** structures the content of a webpage. It is a markup language.

HTML elements define headings, paragraphs, links, images, lists, and other page content. The browser reads HTML and displays the page.

## 2. HTML Document Structure

```html
<!DOCTYPE html>
<!-- lang is an attribute that specifies the language of the page's content. -->
<html lang="en">
  <head>
    <!-- This tag tells the browser which character encoding the HTML document uses. UTF-8 is a widely used character encoding that supports English, many other languages, and a large range of symbols and characters. -->
    <meta charset="UTF-8" />
    <!-- name — Identifies the type of metadata being provided. viewport — Refers to
    the area of the webpage visible to the user. -->
    <!-- Makes the website fit the device's screen width and sets the initial zoom to 100% for mobile-friendly display -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Page</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is my first page.</p>
  </body>
</html>
```

- `<!DOCTYPE html>` tells the browser to use HTML5.
- `<html>` contains the document.
- `<head>` contains metadata; `<title>` sets the browser tab title.
- `<body>` contains the visible page content.

## 3. Text Elements

```html
<h1>Main heading</h1>
<h2>Subheading</h2>
<p>This is a paragraph.</p>
<strong>Important text</strong>
<em>Emphasized text</em>
```

- Headings range from `<h1>` to `<h6>`.
- Use headings to organize content by importance.
- `<strong>` marks important text; `<em>` adds emphasis.

## 4. Lists

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>Open the editor</li>
  <li>Write the HTML</li>
</ol>
```

- `<ul>` creates a bulleted list.
- `<ol>` creates a numbered list.
- `<li>` defines a list item.

## 5. Images and Attributes

```html
<img src="images/photo.jpg" alt="A mountain view" />
```

- `src` specifies the image path or url of image.
- `alt` describes the image for screen readers or if it fails to load.
- Attributes provide extra information about an element.
- `<img>` is a void element, so it has no closing tag.

## 6. Hyperlinks

```html
<a href="https://example.com">Visit website</a>
```

The `<a>` element creates a link, and `href` specifies its destination.

## 7. Structuring a Page

```html
<header>Site heading</header>
<nav>Navigation links</nav>
<main>
  <section>
    <h2>About</h2>
    <p>Page content goes here.</p>
  </section>
</main>
<footer>Copyright information</footer>
```

These elements help divide a page into meaningful sections.

## 8. Semantic HTML

**Semantic HTML** uses elements that describe the purpose of their content.

Examples: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>`.

> Use semantic elements where appropriate instead of using `<div>` for everything. They make code easier to understand and help screen readers or search engines such as google interpret the page.

> In HTML5 use div only when we don't want to attach certain meaning to a certain container.

> Each and every page should have only one h1 heading, it is not necessary but it is a good practice.

> Attribute is nothing but a piece of information describing the element.
