# Day 30: Workshop: Build a Hotel Feedback Form

## Key topics covered:
- [x] `label`
- [x] `input`
- [x] `fieldset`
- [x] legends
- [x] textareas
- [x] `button`


## To review and use 
Upon looking at the example, I can see
- that it has quite a few functions that haven't been covered
  - the sections where there is a reactangular box surrounding the text of that section (I guess similar to heading but different)
  - dropdown
  - freetext comment box that has specific height nad length
 - that I've forgotten about checkbox and the `checked` boolean attribute (though you can tell I do rememeber them, just not how to use them)

Anyway, I'll still follow my approach as usual i.e. do my coding in VS Code and then come back to this workshop - it will look bad/very far away from what it wants me to build

[Ends 09:02 2 Oct 2025]

And here is what I come up with
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Hotel Feedback Form</title>
    </head>
    <body>
        <header>
            <h1>Hotel Feedback Form</h1>
            <p>Thank you for staying with us. Please provide feedback on your recent stay.</p>
        </header>
        <main>
            <section id="pi">
                <!-- This is for Personal Information section but I've done it in <h2> -->
                <h2>Personal Information</h2>
                <form action="">
                    <label for="name">Name (required):</label>
                    <input
                        required
                        id="name"    
                        type="text"                                                
                        placeholder="Ex. John Doe"
                    >
                    <label for="email">Email address (required):</label>
                    <input
                        required
                        id="email"
                        type="email"
                        required
                        placeholder="example@email.com"
                    >
                    <label for="age">Age (optional):</label>
                    <input
                        type="text"
                    >
                </form>
            </section>
            <section id="hotel-qs">
                <!-- This is for the two hotel-related questions but I have no clue what I'm doing below - it's going to be very wrong -->
                <h2>Was this your first time at our hotel?</h2>
                <option type="radio">
                    <p>Yes</p>
                    <p>No</p>
                </option>
                <h2>Why did yuou choose to stat at our hotel? (Check all that apply)
                <option type="checkbox">
                    <p>Social Media Ads</p>
                    <p>Personal Recommendation</p>
                    <p>Location</p>
                    <p checked>Reputation</p>
                    <p>Price</p>
                </option>
                </h2>
            </section>
            <section id="ratings-n-comments">
                <h2>Ratings</h2>
                <!-- I'm conscious whateve I need to use below for the dropdown, there must be a function to show "default option upon customers visiting this page"-->
                <p>How was the service?<dropdown>Excellent, Very good, Good, Satisfactory, Poor</dropdown></p>                
                <p>How was the food<dropdown>Excellent, Very good, Good, Satisfactory, Poor</dropdown></p>
                <form action="">
                    <label for="comments">Other Comments?</label>
                    <input
                        id="comments"
                        type="text"
                    >
                    <button type="button">Submit</button>
                </form>
            </section>
        </main>
        <footer>
            <address>
            </address>
        </footer>
    </body>
</html>
```
You can see it's very wrong in most places.

And I did "cheat" and refer to the notes from Day 28 & 29, as I realised I've forgotten almost all I learnt about `form`. Two key things I referred to: `label name` and the `id` in the `input` element after `label` element.

Redid it following instructions, notes here:\
1. what is "method" attribute? To specify the HTTP method to use when sending the form data. The most common methods are GET and POST. (HTTP comes in more details in later modules)\
   <img width="573" height="160" alt="image" src="https://github.com/user-attachments/assets/e27c29d4-be0d-4efe-8c90-fc7d4ec3345c" />
2. `action` attribute: to specify where the form data should be sent when the form is submitted, **is not** what's covered here in the Form lectures so far and this workshop
3. `fieldset` element to group related inputs together (kind of like `section` or `article` - this is the <h2> in my version above!
   - `legend` element under it to add a caption to describe the group of inputs
4. `name` attribute: to identify form data after it has been submitted to the server
   - what's the difference of this and the `id`?
5. `size`, `type="number"` and the `min` and `max` attraibutes for it within `input`
6. `type="checkbox"`, `value`
7. `select` and `option`
8. `textarea`

[Ends 22:04 3 Oct]

============

Tomorrow - redo it again in VS Code without following instructions.

[Starts 15:36 4 Oct]

Revisit:
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Hotel Feedback Form</title>
    </head>
    <body>
        <header>
            <h1>Hotel Feedback Form</h1>
            <p>Thank you for staying with us. Please provide feedback on your recent stay.</p>
        </header>
        <main>
            <fieldset>
                <legend>Personal Information</legend>
                <label for="full-name">Name (required):</label>
                <input type="text" id="full-name" name="full-name" placeholder="Ex. John Doe" required />
                <label for="email">Email address (required):</label>
                <input type="email" id="email" name="email" placeholder="example@email.com" required />
                <label for="age">Age (optional):</label>
                <input type="number" id="age" name="age" value="age" min="3" max="100" />
            </fieldset>
            <fieldset>
                <legend>Was this your first time at our hotel?</legend>
                <input checked type="radio" id="yes-option" name="yes-option" value="yes-option" />
                <label for="yes-option">Yes</label>
                <input type="radio" id="radio" name="no-option" value="no-option" />
                <label for="no-option">No</label>
            </fieldset>
            <fieldset>
                <legend>WHy did you choose to stay at our hotel? (Check all that appply)</legend>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Social Media Ads</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Personal Recommendation</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Location</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" checked/>
                <label for="hotel-stay">Reputation</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Price</label>
            </fieldset>
            <fieldset>
                <legend>Ratings</legend>
                <label for="service">How was the service?</label>
                <input 
                    type="option"
                />
            </fieldset>
                <label for="comments">Other Comments?</label>
                <input type="textarea" id="comments" name="comments" cols="5" rows="30"/>
                <button type="submit">Submit</button>
        </main>
        <footer>
            <address>
            </address>
        </footer>
    </body>
</html>
```
Still a few things not proficient with:
- `different `type`: text, email, number, button
- `value`: I added the value to the `type="text"` input (name, email, other comments) and it shows in the text box when it first loads. So I had to delete them in all three inputs
- Dropdown: remember it's to do with some `option` things but can't remember how it's done
- for the "Other Comments" section, I do remember the `textarea` type (I think?) and the `cols` and `rows` bit, but when I did it it's not working
- the "submit" button: use `button` or `input`?

End result:
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Hotel Feedback Form</title>
    </head>
    <body>
        <header>
            <h1>Hotel Feedback Form</h1>
            <p>Thank you for staying with us. Please provide feedback on your recent stay.</p>
        </header>
        <main>
            <fieldset>
                <legend>Personal Information</legend>
                <label for="full-name">Name (required):</label>
                <input type="text" id="full-name" name="full-name" placeholder="Ex. John Doe" required />
                <label for="email">Email address (required):</label>
                <input type="email" id="email" name="email" placeholder="example@email.com" required />
                <label for="age">Age (optional):</label>
                <input type="number" id="age" name="age" value="age" min="3" max="100" />
            </fieldset>
            <fieldset>
                <legend>Was this your first time at our hotel?</legend>
                <input checked type="radio" id="yes-option" name="yes-option" value="yes-option" />
                <label for="yes-option">Yes</label>
                <input type="radio" id="radio" name="no-option" value="no-option" />
                <label for="no-option">No</label>
            </fieldset>
            <fieldset>
                <legend>WHy did you choose to stay at our hotel? (Check all that appply)</legend>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Social Media Ads</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Personal Recommendation</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Location</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" checked/>
                <label for="hotel-stay">Reputation</label>
                <input type="checkbox" id="hotel-stay" name="hotel-stay" value="hotel-stay" />
                <label for="hotel-stay">Price</label>
            </fieldset>
            <fieldset>
                <legend>Ratings</legend>
                <label for="service">How was the service?</label>
                <select id="service" name="service">
                    <option value="poor">Poor</option>
                    <option value="satisfactory">Satisfactory</option>
                    <option value="good">Good</option>
                    <option value="very-good">Very good</option>
                    <option value="Excellent" selected>Excellent</option>
                </select>
                <label for="food">How was the food?</label>
                <select id="food" name="food">
                    <option value="poor">Poor</option>
                    <option value="good">Good</option>
                    <option value="very-good">Very good</option>
                    <option value="excellent" selected>Excellent</option>
                </select>
            </fieldset>
                <label for="comments">Other Comments?</label>
                <textarea id="comments" name="comments" rows="10" cols="30"></textarea>
                <button type="submit">Submit</button>
        </main>
        <footer>
            <address>
            </address>
        </footer>
    </body>
</html>
```

----

## What didn't go well
1. Quite a few functions I haven't learnt yet
2. Forgot about checkbox and `checked` attribute
3. Although just learnt Forms in Day 28 and 29, the memory is not that fresh
   > As in, not super sure what the code should be like. Whereas for previous workshops I pretty much remember and almost sure what it should look like
4. Even after finishing it following the instruction inside the workshop i wasn't fully following still (partly because I got sleepy)

## What did go well
1. I still nailed the updated boilerplate
2. Some point near the end of my own trying, I realised that I've missed the `action` attribute of the `form` element (though for all I've been taught, action is always empty - why?)

----

## Suggestions
1. Why are we doing a workshop with functions that haven't been covered in the course so far?
2. 
