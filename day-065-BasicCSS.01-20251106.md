# Day 65: Basic CSS - What is CSS

## Key topics covered
- [x] CSS and its role on the web
- [x] Basic Anatomy of a CSS Rule


## 1. CSS and its role on the web
HTML is the structure of a web page ( foundation and framework of a house), CSS is what makes it look good (paint, wallpaper, and decorations).

CSS works by selecting HTML elements and applying styles to them.
- One of the most powerful aspects of CSS is its ability to create responsive designs, i.e. you can use CSS to make your website look great on any device, whether it's a desktop computer, a tablet, or a smartphone: CSS allows you to adjust layouts, font sizes, and other visual elements based on the screen size of the device viewing the website.
- Another important feature of CSS is its cascading nature. This means styles can be inherited and overridden, allowing for a hierarchical structure of styling.
- Also supports the use of external stylesheets. This means you can keep all your styling rules in a separate file, which can then be linked to multiple HTML pages.
  >  Instead of having to change styles on each individual page, you can make changes in one CSS file that will affect all linked pages.

## 2. CSS Rules
A CSS rule is made up of two main parts: a **selector** and a **declaration** block.
```
selector {
  property: value;
}
```
- selector: a pattern used in CSS to identify and target specific HTML elements for styling.
  - type selectors
  - class selectors
  - ID selectors
  > ```
  > <link rel="stylesheet" href="styles.css">
  > <h1 id="title">Example heading</h1>
  > <h2 class="subheading">Example subheading</h2>
  > <p>This paragraph is not affected by the selector.</p>
  > ```
  > with style.css:
  > ```
  > #title,
  > .subheading {
  >   color: navy;
  > }
  >
  > p {
  >   color: red;
  > }
  > ```
    - `#title`: `id`selector [All id selectors must start with a hash # symbol.]
    - `.subheading`: `class` selector
    - `p`: type selector
  
  
- the curly braces are known as a declaration block. A declaration block applies a set of styles for a given selector, or selectors.
  - Inside the declaration block, you will have a series of declarations. Each declaration consists of a property and a value.
  - The property is the CSS identifier that specifies which feature is being styled.
    > Example: the `background-color` property
  - After each property name, you need to place a colon, and after each value, you should have a semicolon

[Ends 21:17 06 Nov 2025]
