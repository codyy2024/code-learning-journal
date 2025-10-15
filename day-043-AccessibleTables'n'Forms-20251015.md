# Day 43: Theory - How to create accessible tables and forms

## Key topics covered:
- [x] best practices for tables and accessibility
- [x] importance for `input`s to have an associated label

----

## 1. Best practices for tables and accessibility
- Add `caption` right after the opening `table` tag (before the table content)
- Headers (`th`) are a type of data cells (`td`)
- Adding `scope` in `th` to make it clear for screen reader users whether a header is row header or column header
  - 2 most common ones: `col` and `row`
  - must be applied on every `th` opening tag

Accessible table boilerplate

Simple: (not spanning acorss mutiple rows/columns)
```
                <table>
                    <caption>Simple accessible table boilerplate</caption>
                    <thead>
                        <th scope="col">Name</th>
                        <th scope="col">Age</th>
                        <th scope="col">Type</th>
                    </thead>
                    <tbody>
                        <tr>
                            <th scope="row">Nora</th>
                            <td>5</td>
                            <td>Dog</td>
                        </tr>
                        <tr>
                            <th scope="row">Gino</th>
                            <td>2</td>
                            <td>Cat</td>
                        </tr>
                    </tbody>
                </table>
```
More complex: (e.g., spanning across two rows)
```
<table>
                    <caption>Slightly more complex accessible table boilerplate</caption>
                    <tbody>
                        <tr>
                            <td></td>
                            <th scope="col">Name</th>
                            <th scope="col">Age</th>
                        </tr>
                        <tr>
                            <th rowspan="2" scope="row">Dog</th>
                            <th scope="row">Nora</th>
                            <td>5</td>
                        </tr>
                        <tr>
                            <th scope="row">Gino</th>
                            <td>2</td>
                        </tr>
                        <tr>
                            <th rowspan="2" scope="row">Cat</th>
                            <th scope="row">Lulu</th>
                            <td>4</td>
                        </tr>
                        <tr>
                            <th scope="row">Kuku</th>
                            <td>7</td>
                        </tr>
                </table>
```

## 2. Why Is It Important for Inputs to Have an Associated Label?
Labels help people with disabilities, make forms more user-friendly for everyone, and ultimately improve form conversion rates.

Example:
```
<form>
   <label for="name">Your Name</label>
   <input type="text" id="name" />
</form>
```
The `for` attribute of the label element is associated with the `id` of the input element. This connection allows screen readers to announce the label when the input is in a focused state, allowing screen reader users to understand the purpose of the input.

----

## What didn't go well
1. Confused about the second `tr` when you have the first row `th` spanningh across 2 `col`
2. Not sure not sure why mine `captions` are like this:   
   <img width="265" height="422" alt="image" src="https://github.com/user-attachments/assets/81f815d0-2bd1-4608-b616-26e6b8f9b939" />
3. These points are mentioend but not in too mucn detail:
   - try to flatten the table as much as possible to avoid row and column headers that span across multiple cells (some screen readers may not be able to interpret tables with complex structures)
   - for cell width, it's recommended to use relative values, and to avoid using fixed values
   - for cell height, try to avoid defining cell height. This will allow users to adjust the text size to fit their needs.
   - for table width, you should let the browser determine the table width whenever possible, to reduce the need for horizontal scrolling.
4. The last question was a bit odd (label+input when there is error)


## What did go well
1. Better understanding of table element
   
## Suggestions
1. WHY was sandbox not introduced from the very beginning?

=====

[Ends 21:27 15 Oct 2025]
