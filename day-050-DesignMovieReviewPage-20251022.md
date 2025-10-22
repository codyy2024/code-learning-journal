# Day 50: Lab - Desiugn a Movie Review Page

## Key topics covered:
- [x] semantic HTML
- [x] `alt` attributes
- [x] accessible lists
- [x] `aria-hidden`

## 1. What i wrote in VS Code without considering accessibility
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Moview Review Page</title>
    </head>
    <body>
        <main>
            <h1>Moview Review: Rise Beyond</h1>
            <section id="movie-overview">
                <img src="" />
                <p>Rise Beyond is an uplifting drama that tells the story of Ethan Carter, a young man from a small town who dreams of becoming a world-class musician. Facing financial struggles and self-doubt, Ethan embarks on a journey of resilience, guided by his mentor Professor Adams and childhood friend Lena Mitchell. Through setbacks, failures, and moments of triumph, Rise Beyond reminds us that our greatest potential lies beyond our fears.</p>
                <p><b>Movie Rating:</b> (9.2/10)</p>
            </section>
            <section id="movie-cast">
                <h2>Cast Members</h2>
                <li>
                    <ul><b>James Holloway</b> as Ethan Carter</ul>
                    <ul><b>Olivia Sterling</b> as Lena Mitchell</ul>
                    <ul><b>William Lancaster</b> as Professor Adams</ul>
                    <ul><b>Maria Collins</b> as Evelyn Carter (Ethan's Mother)</ul>
                </li>
            </section>
        </main>
    </body>
</html>
```
- I don't know about the stars
- have no idea how to add those accessibility stuff in

Result following instructions:
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Moview Review Page</title>
    </head>
    <body>
        <main>
            <h1>Moview Review: Rise Beyond</h1>

                <img src="https://cdn.freecodecamp.org/curriculum/labs/rise-beyond-2.png" alt="movie poster for rise beyond"/>
                <p>Rise Beyond is an uplifting drama that tells the story of Ethan Carter, a young man from a small town who dreams of becoming a world-class musician. Facing financial struggles and self-doubt, Ethan embarks on a journey of resilience, guided by his mentor Professor Adams and childhood friend Lena Mitchell. Through setbacks, failures, and moments of triumph, Rise Beyond reminds us that our greatest potential lies beyond our fears.</p>
                <p><strong>Movie Rating:</strong><span aria-hidden="true">⭐⭐⭐⭐⭐⭐⭐⭐⭐☆</span>(9.2/10)</p>

                <h2>Cast Members</h2>
                <ul>
                    <li><strong>James Holloway</strong> as Ethan Carter</li>
                    <li><strong>Olivia Sterling</strong> as Lena Mitchell</li>
                    <li><strong>William Lancaster</strong> as Professor Adams</li>
                    <li><strong>Maria Collins</strong> as Evelyn Carter (Ethan's Mother)</li>
                </ul>

        </main>
    </body>
</html>
```
Questions:
- why `strong` over `b`? Rating is not soemthing important or urgent?!
- second time i've seen the use of `span` and `aria-hidden` together - need to revisit `span` to start with
  > `span` is an inline container used to group or style a part of text or inline elements without breaking the flow of content. It has no visual effect by itself — it’s mainly for applying CSS or JavaScript to a specific piece of text. 
- mized the hiearchy structure of `ul` and `li`


## What didn't go well
1. Almost orgot about list
2. Forgot about `alt` initially
3. Still don't get the hang of where and how to add accessibility stuff

## What did go well
Happy with my ability to build these pages now (before adding accessibility attributes).

## Suggestions
Maybe can explain why use certain element over the other - in this case `strong` over `b`

[Ends 21:09 22 Oct 2025]
