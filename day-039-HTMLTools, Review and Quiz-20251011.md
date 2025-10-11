# Day 39: Working with HTML Tools, HTML Table & Forms Review and Quiz

## Key topics covered:
- [x] HTML validators
- [x] DOM Inspector
- [x] broweser developer tools


## HTML validators
A tool that checks the syntax of HTML code to ensure it is valid.
Two common ones
1. [the `w3.org` markup validation service](https://validator.w3.org/#validate_by_input) - most widely accepted one
2. [jasonformatter](https://jsonformatter.org/)

## DOM Inspector
Document Object Model, a tree-like structure that represents the elements on a page. Allows you to inspect and modify the HTML structure of the page you are on.

## DevTools
A set of web developer tools built directly into the browser that helps you debug, profile, and analyze web pages (HTML, CSS, and JavaScript). \
On the web page you are on, right click then click "Inspect"
- Elements tab: shows you the HTML structure of the page you are on
- Console tab: shows you any errors that might be occurring on the page

=====

## Review and Quiz
- "If the input has a button type, the value attribute can be used to set the button text." -- this could've been more useful in one of the workshops when the result was indicating this (which I realised but was not taught in the course before that)
- `name` attribute: used to assign a name to an input field, which serves as the key when form data is submitted.
  > For radio buttons, giving them the same name groups them together, so only one option in the group can be selected at a time.
  > However, for checkboxes that have "Check all that apply", we want to use a different `name` per checkbox ite i.e. input field, so all can be selected if applicable.
- "`size` attribute: used to define the number of characters that should be visible as the user types into the input." -- didn't remember this was the case, and forgot what the use case and purpose is
  > ChatGPT's definition is clearer and less confusing:
  > - It controls how many characters wide the input box appears.
  > - It does not limit how many characters a user can actually type — that’s what maxlength is for.
- "`disabled` attribute: used to specify that an input field should be disabled" -- and what does `disabled` render as output in web page to user?
- "`readonly` attribute: used to specify that an input field is read-only" -- and what does `readonly` render as output in web page to user?
- `button element`: used to create a clickable button. A button can also have a type attribute, which is used to control the behavior of the button when it is activated. Ex. submit, reset, button.

Difference of `disabled` and `readonly`:|
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Buid a Final Exams Table</title>
    </head>
    <body>
        <main>
            <!-- Text input -->
            <input 
            type="text"
            id="name"
            name="name"
            placeholder="e.g. Quincy Larson" 
            size="20"
            minlength="5"
            maxlength="30"
            required
            />

            <!-- Number input -->
            <input 
            type="number"
            id="quantity"
            name="quantity"
            min="2"
            max="10"
            disabled
            />

            <!-- Number input -->
            <input 
            type="number"
            id="quantity"
            name="quantity"
            placeholder="2"
            min="2"
            max="10"
            readonly
            />
            <!-- Button -->
            <input type="button" value="Show Alert" />
        </main>
    </body>
</html>
```
Renders:\
<img width="418" height="35" alt="image" src="https://github.com/user-attachments/assets/29aa60c4-6b4c-4c7f-8bdc-62bfae7d5ebe" />

Render result if I change the `size` to 50: (also shows that `readonly` allows `focused` status but `disabled` doesn't)\
<img width="625" height="42" alt="image" src="https://github.com/user-attachments/assets/2ae3d8e4-4c4f-4bd6-8ef0-8301bf669e4a" />
- Focused state: this is the state of an input field when it is selected by the user.
  > Ex. In screenshot above, it's bolder text field border

Different button types:
```
<button type="button">Show Form</button>
<button type="submit">Submit Form</button>
<button type="reset">Reset Form</button>
```
Same as `input` when `type` is button:
```
<form>
  <input type="button" value="Show Alert" />
</form>
```
<img width="637" height="66" alt="image" src="https://github.com/user-attachments/assets/a0748145-2edb-48de-bb41-c818b7a3cdee" />

