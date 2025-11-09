# Day 68: Basic CSS - What Are Some Default Browser Styles Applied to HTML?

## Key topics cpvered:
- [x] default/"user-agent" browser styles
- [x] Inline, Internal, and External CSS


## 1. Default/"user-agent" browser CSS styles
Provide basic formatting to ensure that HTML elements are displayed in a readable way across all browsers.
> anchor `a` style is blue and underlined
> `hr` is a horizontal line with space before and after it

## 2. Inline, Internal, and External CSS
### 2.1 Inline CSS
- written directly within an HTML element using the style attribute
- It applies styles to a specific element
- generally used for quick, one-off styles or to override other styles for a specific element, but should be avoided as it clutters the HTML file

### 2.2 Internal CSS
- written within the style tags inside the `head` section of an HTML document
- It applies styles to the entire page and is useful when you need to style a single document
- best used when you need to apply styles to a specific page rather than across multiple pages
- useful for single-page websites or when the styles don’t need to be reused elsewhere.
  - not promoting reusability across multiple pages.
  - like inline CSS, it mixes HTML and CSS,
### 2.3 External CSS
- written in a separate .css file and linked to the HTML document using the link element in the head section.
- It allows you to style multiple pages consistently and is the preferred method in professional web development.
- External CSS is ideal for large projects where you want to maintain a consistent style across multiple pages.

[Ends 21:05 9 Nov 2025]

