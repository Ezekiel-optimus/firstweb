# First Web

A beginner-friendly static landing page built with plain HTML and CSS. The project is a hands-on introduction to structuring a webpage, styling it with Flexbox, and adding simple interactive states without a JavaScript framework.

## Overview

The page presents a fictional product and includes a top navigation, a hero area with a sign-up button, a four-image content section, a quotation, a second call to action, and a footer. Its dark header, blue accents, and image gallery make it a compact exercise in building a complete page from scratch.

## Project Structure

```text
firstweb/
├── index.html          # Page content and HTML structure
├── styles.css          # Layout, colors, typography, and hover states
├── noper.png           # Navigation logo
├── preview.webp        # Hero image
├── coding.jpg          # Gallery image
├── heading-img.jpg     # Gallery image
├── Transformers.jpeg   # Gallery image
├── Capture.PNG         # Gallery image
└── computer.jpg        # Additional image asset, not currently displayed
```

## How the Page Is Built

### HTML structure

`index.html` contains the page content and links to the stylesheet. The document is divided into familiar regions:

- `<header>` holds the logo, navigation, and hero content.
- `<main>` groups the gallery, quotation, and call-to-action sections.
- `<footer>` displays the site name and year.
- Headings, paragraphs, links, buttons, images, and `<cite>` provide the content for each section.

The navigation links currently use `href="#"`, and the sign-up buttons are visual examples rather than working forms or links.

### CSS styling and layout

`styles.css` styles the page by element and class. Flexbox is used for the navigation, hero, image gallery, and call-to-action banner. Other rules set spacing, typography, colors, borders, and image dimensions. Hover selectors change the appearance of buttons, images, and navigation links when the pointer is over them.

The design is currently fixed around a desktop layout: the main flex rows do not wrap, and the stylesheet does not include media queries. This makes responsive design a useful next exercise.

## What You Can Learn

- **HTML foundations:** document metadata, stylesheet linking, semantic page regions, headings, links, buttons, images, and text content.
- **CSS selectors:** element selectors, class selectors, descendant selectors, and pseudo-classes such as `:hover`.
- **Flexbox:** arranging content in rows, distributing space, and controlling gaps and alignment.
- **Visual styling:** using color, typography, spacing, borders, rounded corners, and shadows to create a consistent visual theme.
- **Asset management:** keeping image files alongside a page and referencing them from HTML.
- **Iteration:** identifying the difference between a visual prototype and a functional, accessible, responsive website.

## Run Locally

No package manager, build step, or JavaScript runtime is required. From the project directory, start Python's built-in static server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` in your browser. Serving the project from its root ensures the page's root-relative image paths (for example, `/preview.webp`) resolve correctly. Alternatively, use a VS Code local preview extension configured to serve the project root.

## Ideas for Improvement

- Add media queries and flexible sizing so the layout works on mobile screens.
- Add descriptive `alt` text to the images and ensure the page has a clear heading hierarchy.
- Replace placeholder navigation links and connect the sign-up buttons to a form or destination.
- Improve keyboard focus styles and check text/background contrast.
- Consider replacing root-relative image paths such as `/preview.webp` with paths relative to the project, such as `preview.webp`, for easier deployment under a repository subpath.
- Use the currently unused `computer.jpg` in the page or remove it if it is not needed.

## Technologies

- HTML5
- CSS3

There are no external dependencies.