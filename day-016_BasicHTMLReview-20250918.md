# Day 16: Basic HTML Review before being quizzed

New things picked up

## <ins>Elements</ins>

Building blocks of an HTML document (headings, paragraphs, links images, videos etc)
  
Syntax:
- Non-void elements `<element>Content</element>`
- Void elements __cannont__ have any content, `<element>` or `<element/>`
  > E.g., `<img>`, `<meta>` or `<img/>`, `<meta/>`

## <ins>Attributes</ins>

A **value** placed inside the **opening** tag of an HTML element;

Aditional info (noun) of the element OR how the element should behave (verb)

Syntax:   
|   | Non-boolean attribute | Boolean attribute |
| --- | --- | --- |
| Non-void element | `<element attribute="value">Content</element>` | `<element attribute>Content</element>` (or not present, means == false) |
| Void element | `<element atttribute="value">` | `<element atttribute>` (or not present, means == false)|
> Example of boolean attributes: `disabled`, `readonly`, `required`

## Common HTML elements
- Heading: h1 to h6
- `p`
- `body`: **content** of HTML document
- `section`: semantic element to divide content into smaller and meaningful sections
- `div`: non-semantic element used as a generic container to hold other HTML elements
- `a`: src, href and target attributes

(To be continued tomorrow)
