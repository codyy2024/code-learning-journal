# Day 24: Lecture - Working with Specialized Semantic Elements

## Key topics covered
- [x] How to Display mathematical equations and chemical formulas in HTML
- [x] How to represent computer code in HTML
- [x] How to use U, S and Ruby elements

---

## 1. How to Display mathematical equations and chemical formulas in HTML
### 1.1 Superscript
Common uses
- exponents, e.g., `<p>2<sup>2</sup> (2 squared) is 4.</p>` renders as **2<sup>2</sup>**
- superior lettering, to indicate abbreviations, e.g., `<p>Monseigneur is often written as <strong>M<sup>gr</sup></strong>.</p>` renders as "Monseigneur is often written as **M<sup>gr</sup>** (In English, superior letters are reserved for use with ordinal numerals, as in 1st, 2nd, 3rd, etc.) 
- ordinal numbers: e.g. `<p>1<sup>st</sup> of October` renders as **1<sup>st</sup> of October**

[The superscript element should only be used for typographical reasons. If you want style a piece of text with a raised baseline, then you should use CSS instead]
### 1.2 Subscript
Common uses:
- chemical equations, e.g., `<p>CO<sub>2</sub></p>` renders as **CO<sub>2<sub>**
- variable script, e.g., `<p><em>N<sub>i</sub></em>` renders as ***N<sub>i</sub>*** - this is my own explanation/understanding of what "variable script" means here, unsure if currect or not
- footnote: big questions here - aren't footnotes superscript instead?? For example:<img width="577" height="161" alt="image" src="https://github.com/user-attachments/assets/64177473-d223-4eaa-8fa0-f35bcf066ee2" />

## 2. How to represent computer code in HTML
The default styling for content inside the `code` element is a monospaced font.
### 2.1 Inline code
Use the `code` element to for short inline snippet of code inside text. 

Example:
```
<p>
  To set the text color to blue in CSS, use the following code:
  <code>color: blue;</code>
</p>
```
### 2.2 Multiple lines of code
Use the `pre` (preformatted text - what is this??) and `code` elements to display longer/multiple lines of code snippets. Example:
```
<pre>
  <code>
    body {
      color: red;
    }
  </code>
</pre>
```

===

Renders:   
<img width="489" height="114" alt="image" src="https://github.com/user-attachments/assets/e2869255-fddf-4d8b-90de-41f7d71f1075" />

## 3. How to use U, S and Ruby elements
### 3.1 `u` element
Unarticulated annotation element used to represent inline text that has non-textual annotation applied.

The default styling for the u element is a black underline underneath the text. Visually it looks the same as underline.

Example:
```
<p>
  You can use the unarticulated annotation element to highlight
  <u>inccccort</u> <u>spling</u> <u>issses</u>.
</p>
```
Renders:   
<img width="569" height="37" alt="image" src="https://github.com/user-attachments/assets/99ba221c-e100-471f-a3c5-5b2cee8d4c8b" />

### 3.2 `s` element
The strikethrough element used to represent when text is no longer accurate or relevant.

### 3.3 `ruby`element
Represents small text shown above or below the main text. It is typically used to show the pronunciation of East Asian characters.

Example:
```
<ruby> 明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp> </ruby>
```
- the `rp` element: ruby fallback parenthesis element used as a fallback for browsers lacking support for displaying ruby annotations. (What is ruby annotation?)
- the `rt` element: ruby text element used to indicate text for the ruby annotation. This text is usually used for pronunciation, or translation details in East Asian typography.

Renders:   
<img width="69" height="61" alt="image" src="https://github.com/user-attachments/assets/d678f798-2956-4e2c-a0f8-ce8dfe0b4897" />

Another example:
```
<ruby>
  学 <rp>(</rp><rt>xu&#233;</rt><rp>)</rp>
  生 <rp>(</rp><rt>sh&#275;ng</rt><rp>)</rp>
</ruby>

OR

<ruby>
  学 <rp>(</rp><rt>xu&eacute;</rt><rp>)</rp>
  生 <rp>(</rp><rt>sh&emacr;ng</rt><rp>)</rp>
</ruby>
```
Renders:(need to learn the [numeric code/HTML entities](https://www.w3schools.com/charsets/default.asp))   
<img width="104" height="66" alt="image" src="https://github.com/user-attachments/assets/81b7f21a-6e41-4512-b390-8668ea1d270f" />

---

## What didn't go well
1. This lecture really didn't go deep into explaining the different usage scenarios - I had to do a lot of googling to find what some of those are (variable script? footnote being subscript? non-contexual annotation? ruby?)
2. Esp. in this lecture, a view-rendering-result-as-you-edit thing would be **very** useful - I had to use .md syntax to show what it'd render in HTML
3. The last question for [superscript](#11-superscript) seems wrong/confusing:<img width="762" height="368" alt="image" src="https://github.com/user-attachments/assets/5f9997a1-b6b2-4dd2-bf3a-2737d5dfda25" /> 

## What did go well
1. Try to be more inquisitive which I kind of lost a bit during the last few days.

---

## Suggestions
1. Explain all that's covered clearly, or link to external sources. OR at least let the learners know they will be covered later down the line so don't need to worry too much for now.
2. Give thorough examples


[Ends 21:26 26 Sep 2025]
