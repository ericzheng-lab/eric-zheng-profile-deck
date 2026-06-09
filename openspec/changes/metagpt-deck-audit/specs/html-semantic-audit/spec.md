## ADDED Requirements

### Requirement: HTML document SHALL have proper lang attribute
The `<html>` tag SHALL include `lang="en"` for screen reader compatibility.

#### Scenario: Missing lang attribute
- **WHEN** the HTML document is parsed
- **THEN** the `<html>` tag SHALL have `lang="en"` attribute

### Requirement: HTML SHALL have proper meta tags
The document SHALL include viewport meta tag, charset meta tag, and description meta tag.

#### Scenario: Missing meta tags
- **WHEN** the HTML document is loaded
- **THEN** it SHALL have `<meta charset="UTF-8">`, `<meta name="viewport" ...>`, and `<meta name="description" ...>`

### Requirement: Heading hierarchy SHALL be sequential
Headings SHALL follow sequential order (h1 → h2 → h3) without skipping levels.

#### Scenario: Heading hierarchy check
- **WHEN** the document heading structure is analyzed
- **THEN** there SHALL be exactly one `<h1>` element and all `<h2>` elements SHALL be direct children of the document, with no `<h3>` nested under `<h2>` without intermediate `<h3>`

### Requirement: Slide structure SHALL use semantic HTML
Each slide SHALL use semantic HTML elements where appropriate (e.g., `<article>`, `<section>`, `<nav>`).

#### Scenario: Slide semantics
- **WHEN** the slide structure is analyzed
- **THEN** each slide SHALL use `<section>` or `<article>` elements with appropriate ARIA roles

### Requirement: Lists SHALL use proper list elements
Content that represents a list of items SHALL use `<ul>`, `<ol>`, or `<dl>` elements.

#### Scenario: List elements check
- **WHEN** the document is analyzed for list-like content
- **THEN** all list-like content SHALL use proper list elements instead of divs or paragraphs
