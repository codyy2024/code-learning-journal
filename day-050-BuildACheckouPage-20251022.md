# Day 49: Lab - Build a Checkout Page

## Key topics covered
- [x] `alt` attributes
- [x] ARIA roles

### 1. I started with the accessibility not built in like so:
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Checkout Page</title>
    </head>
    <body>
        <header>
            <h1>Checkout</h1>
        </header>
        <main>
            <h2>Your cart</h2>
            <img src="" 
            
            />
            <p>Left-handed spoon</p>
            <p>£29.99</p>
            <h2>Payment Information</h2>
            <label for="cardholder-name">Cardholder Name *</label>
            <input type="text" id="cardholder-name" required >
            <br/>
            <label for="card-no">Card Number *</label>
            <input type="number" id="card-no" required minlength="16" maxlength="16" />
            <p>Please enter your 16-digit card number without spaces or dashes.</p>
            <label for="expirey-date">Expiry Date *</label>
            <input type="text" id="expirey-date" required placeholder="MM/YY">
            <br/>
            <label for="cvv">CVV *</label>
            <input type="number" required minlength="3" maxlength="4" />
            <br/>
            <button type="submit" value="Place Order">Place Order</button>
        </main>
    </body>
</html>
```
Two issues noticed:
1. For the Card Number and CVV input fields, I've set the `type` to `number`, but it seems to render as choosing to type in a single digit number (or natural numbers? don't know how to explain this)\
   <img width="248" height="46" alt="image" src="https://github.com/user-attachments/assets/8c153564-bbb8-4999-bdb0-c257bb887188" />\
   Makes me wonder whether we should set the `type` to `number` ONLY when we're asking users to input single digit?
2. I first had the `button` element like so `<button type="submit" value="Place Order"></button>` as vaguely remember that the `value` attribute can be what's shown as the button text. But it doesn't seem to be the case:\
   <img width="311" height="78" alt="image" src="https://github.com/user-attachments/assets/ac3f9ad9-81b2-4e5e-a0cd-c617de685e85" />

### 2. Then trying to remember the accessibility pratices regarding `alt` and ARIA and apply it in the above
CANNOT REMEMBER ANYTHING!\
(I mean I remember  `aria-rol` and `aria-labelledby` but thats it.)

So here it is following thr instructions:
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Checkout Page</title>
    </head>
    <body>
        <main>
            <h1>Checkout</h1>
            <section id="your-cart">
                <h2>Your Cart</h2>
                <img src="https://cdn.freecodecamp.org/curriculum/labs/cube.jpg" 
                alt="a stainless steel spoon on top of a table"
                />
                <p>Left-handed spoon</p>
                <p>£29.99</p>
            </section>
            <section id="payment-info">
                <h2>Payment Information</h2>
                <form>
                    <label for="card-name">Cardholder Name <span aria-hidden="true">*</span></label>
                    <input type="text" id="card-name" name="card-name" required >
                    <br/>
                    <label for="card-number">Card Number <span aria-hidden="true">*</span></label>
                    <input type="text" id="card-number" name="card-number" required minlength="16" maxlength="16" aria-describedby="card-number-help"/>
                    <p id="card-number-help">Please enter your 16-digit card number without spaces or dashes.</p>
                    <label for="expiry-date">Expiry Date <span aria-hidden="true">*</span></label>
                    <input type="text" id="expiry-date" required placeholder="MM/YY">
                    <br/>
                    <label for="cvv">CVV <span aria-hidden="true">*</span></label>
                    <input type="text" id="cvv" required minlength="3" maxlength="4" />
                    <br/>
                    <button type="submit" value="Place Order">Place Order</button>
                </form>
            </section>
        </main>
    </body>
</html>
```

A few things:
- thought of `section` but slipped off my mind in the end
- completely forgot about `form` then the `label` and `input` elements
- completely forgot about `name` attribute in the `input` element, and what it actually means/does at the backend
- even though i finished it following the instructions, I still
  - don't know why the need to `<span aria-hidden="true">*</span>`
  - not sure if `aria-describedby` was covered (somehow I only remember `aria-labbeledby`.)


## What didn't go well
Completely forgot about how to use the ARIA related attributes.

## What did go well
- Was still able to build this without the accessibility factored in *okay* - forgot about `section`,  `form` and `name`

## Suggestions
The instruction on the `aria-describedby` was rather confusing - I added like this instead for the firt time:
```
<label for="card-number">Card Number <span aria-hidden="true">*</span></label>
<input type="text" id="card-number" name="card-number" required minlength="16" maxlength="16" />
<p id="card-number-help" aria-describedby="card-number">Please enter your 16-digit card number without spaces or dashes.</p>
```

[Ends 09:04 22 Oct 2025]


