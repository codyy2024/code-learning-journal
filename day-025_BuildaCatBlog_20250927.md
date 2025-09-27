# Day 25: Workshop - Build a Cat Blog Page

## Key topics covered:
- [x] build an HTML only blog page
- [x] use semantic elements `main`, `nav`, `article` and `footer` elements

[Big question here: unless my my mempry is completely messed up, I don't think the last three have been covered in much detail. Maybe `footer` was covered specifically and a bit more than the others, but `nav` and `article` were only introduced as part of other topics/elements. So if I'm honest, I'm not that comfortable/confident about this workshop. But let's see.]

----

- Unsure really where `nav` lives: in the `head` element, or in the `main` element in `body`?
> Answer: in `header` which is under `body` before `main`
- Unsure about how to use `section` - I mean I know how to use the elements, just not 100% sure what the best practise/meaning behind this
> Answer: use it in conjunction with `id` to refer to later
- Unsure about the Phone, Email, and Address sections in the footer
> Answer: don't forget about `address` element
- Don't remember the `header` element inside `body` element at all
> Asnwer: in general it's body > header (h1, intro paragraph, image, nav), main, and footer
- Forgot about using `id` for e.g., section (and id needs to be unique i.e. each one should only appear once)
- Don't know how to use `article` either
- Good that I still have a good grasp of boilerplate and the usage of `figure` and the `img` and `figcaption` elements in it.
- Glad the `ul` nad `li` under it comes to life to me while I was writing the blog page outside of freeCodeCamp in Visual Studio Code, but unsure if it sits at the same level as `p`, or needs to sit under `p`

====

## Workshop end result:
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Mr. Whiskers' Blog</title>
    <meta charset="UTF-8" />
  </head>
  <body>
    <header>
      <h1>Welcome to Mr. Whiskers' Blog Page!</h1>
      <figure>
        <img
          src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/1.jpg"
          alt="a cat in the garden"
        />
        <figcaption>Mr. Whiskers in the Garden</figcaption>
      </figure>
      <nav>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#posts">Posts</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section id="about">
        <h2>About</h2>
        <p>
          Hi there! I'm Jane Doe, a passionate writer who finds endless inspiration in the antics of my beloved cat, Mr. Whiskers.
        </p>
        <p>
          His playful nature and boundless energy keeps me on my toes. I love him so much.
        </p>
      </section>
      <section id="posts">
        <h2>Posts</h2>

        <article>
          <h3>Mr. Whiskers' First Day Home</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            quod, voluptates, quae, quos quibusdam dolorum quia nemo repudiandae
            quidem voluptatum quas. Quisquam quod, voluptates, quae, quos
            quibusdam dolorum quia nemo repudiandae quidem voluptatum quas.
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            quod, voluptates, quae, quos quibusdam dolorum quia nemo repudiandae
            quidem voluptatum quas. Quisquam quod, voluptates, quae, quos
            quibusdam dolorum quia nemo repudiandae quidem voluptatum quas.
          </p>
        </article>
        <article>
          <h3>Mr. Whiskers' First Bath</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            quod, voluptates, quae, quos quibusdam dolorum quia nemo repudiandae
            quidem voluptatum quas. Quisquam quod, voluptates, quae, quos
            quibusdam dolorum quia nemo repudiandae quidem voluptatum quas.
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            quod, voluptates, quae, quos quibusdam dolorum quia nemo repudiandae
            quidem voluptatum quas. Quisquam quod, voluptates, quae, quos
            quibusdam dolorum quia nemo repudiandae quidem voluptatum quas.
          </p>
        </article>
        <article>
          <h3>Mr. Whiskers' First Birthday Party</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            quod, voluptates, quae, quos quibusdam dolorum quia nemo repudiandae
            quidem voluptatum quas. Quisquam quod, voluptates, quae, quos
            quibusdam dolorum quia nemo repudiandae quidem voluptatum quas.
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
            quod, voluptates, quae, quos quibusdam dolorum quia nemo repudiandae
            quidem voluptatum quas. Quisquam quod, voluptates, quae, quos
            quibusdam dolorum quia nemo repudiandae quidem voluptatum quas.
          </p>
        </article>
      </section>
    </main>
    <footer>
        <section id="contact">
            <h2>Contact</h2>
            <address>
                <p>Phone: <a href="tel:5555555555">555-555-5555</a></p>
                <p>Email: <a href="mailto:fake@email.com">fake@email.com</a></p>
            </address>
        </section>
    </footer>
```

## What I created before the workshop:
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>The Life of Codes and Corbs</title>
        <link>
    </head>
    <body>
        <main>
            <h1>The Life of Codes and Corbs in the UK</h1>
            <figure>
                <img src="https://github.com/user-attachments/assets/64177473-d223-4eaa-8fa0-f35bcf066ee2" alt="A black dog sitting under the sun in the garden" >
                <figcaption>Scardicat Corby</figcaption>
            </figure>
            <h2>About</h2>
            <p>Codes is a coding newbie <a href="https://codyy2024.github.io/code-learning-journal/" target="_blank">learning to code</a>. Corby is a UK newbie learning to not bark and have a go at every squirrel, bird, cat, fox and pigeon that passes by the fence.</p>
            <p>Corby is otherwise a lovely, cute and gentle dog, that went through some trauma so had some trusting problems with both human and other dogs. He's come a long way - both geologically from Romania and psychologically since arriving in the UK.</p>
            <p>I'd like to share and keep a log of the memories of him with us.</p>
            <section>
                <h2>Pawsts</h2>
                <h3>Corby's Arrival Day</h3>
                <p>He slept on the floor.</p>
                <h3>Corby's First Couple of Weeks</h3>
                <p>We slept on the floor with him in turn for a couple of weeks downstairs.</p>
                <p>He wouldn't pee or poo when it was windy. And there was one time when he woke me up to say "I need to pee", but then couldn't pee because it was too windy and disturbing; Then another night he was too scared by the umbrella I was holding to keep the rain from him. HE also would hide in the rosemary bush and refused to come out or move sometimes.</p>
                <h3>Corby's first couple of months</h3>
                <p>Slowly building his confidence.
                    <ul>
                        <li>Dog behaviourist;</li>
                        <li>Jumping onto the sofa;</li>
                        <li>Took the apple from the coffe table;</li>                 
                    </ul>
                </p>
                <h3>Corby Settling In</h3>
                <p>Can't rememebr for how long, but was really glad to see Corby coming out of his shell.</p>
                    <ul>
                        <li>Showing playfulness;</li>
                        <li>Showing his belly;</li>
                        <li>Took the strawberry from the basket in the garden;</li>
                        <li>First time (we believe) seeing snow</li>
                    </ul>
            </section>
        </main>

        <footer>
            <p>Phone: <a href="tel:447778274709">447778274709</a></p>
            <p>Email: <a href="mailto:yi.yang813@gmail.com">yi.yang813@gmail.com</a></p>
        </footer>
    </body>
</html>
```

What I then updated to:
```

```
