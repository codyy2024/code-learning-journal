# Day 22 Lecture - Working with Text and Time Semantic Elements
Learn about the importance of semantics in conveying meaning for text and time-related content including the time, blockquote elements and more.

## Key topics covered
- [x] Block and inline quotes in HTML
- [x] Display abbreviation in HTML
- [x] Display address in HTML
- [x] Display times and dates in HTML

---

## 1. How do block and inline quotes work in HTML? (Non-void elements)
- Use block quotes for extended quotations from other sources
- Use inline quotes for short quotations (a few words) from other sources that should be part of existing paragraphs

### 1.1 Block quotes `blockquote`
Example 1
- double quotation marks `"` added manually by **YOU** (not automatically added)
- `cite` attribute
  - URL behind the scene (does not show in browsaer);
  - helpful for giving screen readers and search engines more information about the quote
- indented
```
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  "Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?"
</blockquote>
```

Example 2: mutiple paragraphs (not adding quotation marks)
```
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  <p>Build your projects. Show them to your friends. Build projects for your friends.</p>
  <p>Build your network. Help the people you meet along the way. What goes around comes around. You'll get what's coming to you.</p>   
  <p>It is not too late. Life is long.</p>
  <p>You will look back on this moment years from now and be glad you made a move.</p>
</blockquote>
```
Example 3: `cite` element inside `blockquote` element
- Mark up the title of a referenced creative work (boik, film etc.)
_**Q**: How is this different from `i` or `em`, visually?_
```
<div>
  <blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?
  </blockquote>
  <p>—Quincy Larson, <cite>How to Learn to Code and Get a Developer Job [Full Book].</cite></p>
</div>
```

### 1.2 inline quote `q`
- Most modern browsers will add the double quotation marks automatically
- Quotes not indented but as parf of the paragraph
Example 1: 
```
<p>
  As Quincy Larson said,
  <q cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Momentum is everything.
  </q>
</p>
```
<br></br>
\===\
Render results:

<img width="884" height="274" alt="chrome_goFhCie5Sz" src="https://github.com/user-attachments/assets/125e0266-5ef4-4c49-b85a-2eca8024bb3c" />


[Ends 09:22]

## 2. How do you display abbreviation in HTML?

## 3. How do you display address in HTML?

## 4. How do you display times and dates in HTML?
