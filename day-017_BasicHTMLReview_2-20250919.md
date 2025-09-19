# Day 19: Basic HTML Review - Part 2

I have to admit - yesterday to today has been quite a day: woken up by my little one several times (she's got a cold and runny/stuffy nose), a driving lesson as usual from 7am to 9am, then work pretty non stop till 5pm.

I will stick my self-descipline, but maybe reduce the time. So there will be at least Part 3, maybe more. Let's see.

(continued from Day 16)
- `ul` and `ol`, and `li` within it as a child element
- `em`: amphasise
- `strong`: emphasis on text with urgency and seriousness
- `figure` and `figcaption`:
  - `figure`: group content like images and diagrams (This definition is **new** to me, but makes sense.)
  - `figcaption`: caption for content in `figure`
- `main`: child under `body` to represent the main content
- `footer`: usually bottom of the HTML document to contain copyright info ir important links (This definition is **new** to me, but makes sense.)

## Identifiers and Grouping
- `id` attribute: unique identifiers for HTML elements
  - Can **not** have space in its value (i.e. id name), e.g. `<div id="redbox"></div>` or `<div id="red-box"></div>` CANNOT be `<div id="red box"></div>`
- `class`: group elements for styling and behaviour
  - can reuse the same class name throughout an HTML document
  - can have spaces
  > Example: `<div calss="red box"></div>` or `<div calss="red-box"></div>` or  `<div calss="redbox"></div>`

## Special Characters and Linking
- entities: a set of characters to represent a reserved character in HTML (or, to show the content instead of it being back end code (not-showing to front end user)
  - different types: hex, numeric, ??
  - format:
    - hex: ??
    - numeric: &xxx;
    - ??
  > Example: `<p>This is an &lt;img /&gt; element</p>` will render out as "This is an <img> element" to end user when they browese this web page; however if you write it as `<p>This is an <img> element</p>` it will render out as "This is an element" (<ins>not too sure</ins>)
- `link` element and `rel` attribute: link to external resources like stylesheets and site icons.
  - `rel`: specify the relationship between the linked resource and the HTML document
  - `href`: specify the location of the URL for the external resource.
  > **Q**: `src` and `href`  seems quite similar and confusing, what's the difference? (href is for link other than images, src is for a image, video and audio?)
- `script` element
  - write the JavaScript directly in the HTML document (not recommended)
    > Example:
    ```
    <body>
    <script>
      alert("Welcome to freeCodeCamp");
    </script>
    </body>
    ```
  
  - create the JavaScript in an external file and then links to it
    > Example:
    ```
    <script src="path-to-javascript-file.js"></script>
    ```

    ## Boilerplate and Encoding
    (To be continued)
