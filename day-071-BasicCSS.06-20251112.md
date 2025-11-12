# Day 71: Basic CSS -  Inline and Block-Level Elements

## 1. HTML and CSS elements can be divided into two categories: block-level elements and inline elements
### 1.1 Block-level elements
- Elements that take up the full width available to them by default, stretching across the width of their container.
- Block-level elements have the CSS property `display: block;` applied by default. This property ensures that the element stretches to fill the container's width and appears on a new line.
- Common block-level elements: headings i.e. `h1` to `h6`, `p`, `section`, `div`, `ul`, `ol`
- Best usage scenario: Block-level elements are ideal when you want content to stack vertically, such as paragraphs, sections, or larger blocks of content. They're commonly used to define the layout and structure of a webpage.

Example:\
<img width="1264" height="125" alt="image" src="https://github.com/user-attachments/assets/97200634-4494-4d94-9bc0-e6abd59ade13" />
- both `p` elements will take up the full width of its container, which in this case is the `body` element.


### 1.2 Inline elements
- only take up as much width as they need
- inline elements have the CSS property `display: inline;` applied by default. This property ensures that the element remains within the flow of the content and does not break onto a new line.
- Common inline elements: `span`, `a` and `img`
- Best usage scenario: for styling smaller portions of text or content within a line, such as emphasizing a word, creating hyperlinks, or applying specific styles to parts of a paragraph.

Example:\
<img width="1034" height="117" alt="image" src="https://github.com/user-attachments/assets/496e06b2-926a-41a8-b31e-8df4a32fca2a" />
- As you can see, the span element only takes up as much space as the word "red" and does not push the following content to a new line.


## What did go well
1. Instantly, I was recapping in my head:
   - If based on semantic or not, then HTML can be divided into two categories: semantic and non-semantic/presentational elements
   - If divided based on closing or not, then HTML can be divided into these two categories instead: self-closing vs. non-self-closing elements


[Ends 09:10 12 Nov 2025]
