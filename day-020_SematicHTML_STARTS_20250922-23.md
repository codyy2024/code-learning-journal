# Day 20: Lectures - Importnance of Semantic HTML 
Self-revise before even starting: semantic element in HTML represents an element that has a meaning that human and machine can read/understand easily.

An example of semantic element is `section`, and non-semantic is `div`

Two immediate questions after reading the lecture summary: 
1. What is "presentational" HTML?
2. What does semantic HTML get anything to do with "good structural hierarchy"?

---

Part 1 - finished 22 Sep

---

## 1. Why should you care about semantic HTML?
Semantics are the meaning of words, or phrases, in a language. The semantic meaning of an element refers to what special information that element conveys.
> The semantic meaning of a p element, for example, is a paragraph of text
> > Most elements have semantic meaning (`div` is one of the very few that doesn't) - had this definition been mentioned earlier, it would have made the previous introduction to semantic elements much more easier.
Why is semantic element important?
- improves accessibility (ensure the best experience for users with assistive technology like screen readers)
- improves SEO (your search rankings)
- improves your development experience (e.g., edit the `nav` element directly instead of sifting through a bunch of developments (not quite sure what this means)
## 2. Why is it important to have good structural hierarchy?
Most important aspect: use heading elements `h1`, `h2`, `h3` etc.
  - `h1`: top level heading
    - comes before all of your content
    - **rarely** have it more than once
  - `h2`: your subheading
    - always come after your h1
    - might come after some introductory text/`p`
    - can have multiple
  - and so on
  - should never skip, e.g., directly from `h1` to `h3` (It very makes sense but **WHY**??)

The right hierarchy
- is important for accessibility
  - determine how assistive technologies (Screenreaders) parse and announce that web page to the user
- is important for SEO
  - Search engines use automation to parse the content of your web page and determine when and where it should show up in results
- mean your HTML may not even be technically valid with incorrect structure

---

Part 2 - finished morning of 23 Sep

---

## 3. What is the difference between presentational and semantic HTML?
Simply put: presentational elements are mostly deprecated elements that focus on **appearance**, whi8le semantic elements are the best practise in modern days that **describe the content**.


