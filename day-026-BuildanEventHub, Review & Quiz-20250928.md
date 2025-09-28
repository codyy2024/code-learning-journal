# Day 26: Lab - Build an Event Hub

## Key topics covered:
- [x] Review what we learnt in Day 25 about the `header`, `nav` and `article` etc.

----
- Kind of forgot about the `date` element and the specific data + time format we should follow.
- 
----

End result - again I didn't read the instructions and follow them to write the HTML. I just looked at the preview of the example, and wrote the code in Visual Studio Code:
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <title>Event Hub</title>
    </head>
    <body>
        <header>
            <h1>Event Hub</h1>
            <nav>
                <ul>
                    <li><a href="#upcoming-events">Upcoming Events</a></li>
                    <li><a href="#past-events">Past Events</a></li>
                </ul>
            </nav>
        </header>
        <main>
            <section id="upcoming-events">
                <h2>Upcoming Events</h2>
                <article>
                    <h3>AI & Machine Learning Conference 2024</h3>
                    <p>Join us for a deep dive into the latest advancements in artificial intelligence and machine learning. Industry leaders will share insights and case studies on how AI is transforming various sectors.</p>
                    <p>Date: August 10, 2024</p>
                </article>
                <article>
                    <h3>Web Development Bootcamp</h3>
                    <p>A hands-on workshop designed for developers looking to enhance their skills in modern web technologies including React, Node.js, and GraphQL. Perfect for both beginners and experienced developers.</p>
                    <p>Date: September 5, 2024</p>
                </article>
            </section>
            <section id="past-events">
                <h2>Past Events</h2>
                <article>
                    <h3>Cybersecurity SUmmit 2024</h3>
                    <p>An event focusing on the latest trends and threats in cybersecurity. Experts discussed strategies for protecting data and ensuring privacy in an increasingly digital world.</p>
                    <p>Date: June 15, 2024</p>
                    <figure>
                        <img src="https://cdn.freecodecamp.org/curriculum/labs/past-event1.jpg" alt="an old computer">
                    </figure>
                </article>
                <article>
                    <h3>Blockchain Expo 2024</h3>
                    <p>A comprehensive event covering the future of blockchain technology. Topics included decentralized finance (DeFi), smart contracts, and the impact of blockchain on various industries.</p>
                    <p>Date: July 20, 2024</p>
                        <img src="https://cdn.freecodecamp.org/curriculum/labs/past-event2.jpg" alt="computer generated image">
                </article>
            </section>
        </main>
    </body>
</html>
```
Notice that the `img` with no caption, I've still used the `figure` element and wrote the `img` element under it with no `figcaption`. However the render result seems different - the `figure` element seems to indent the whole section under `figure` slightly, while if you put `img` directly after the last `p`, it's not indented. So I've amended the second image to remove `figure` - and it proved me right. 

## Semantic Elements Review
1. The 15th question could have been a very simple but clear differentiation between `b`, `strong`, `i` and `em` (in the order of the 4 choices of the question)
   <img width="679" height="339" alt="image" src="https://github.com/user-attachments/assets/808eb9da-d32a-4072-b84e-ab6517b8dbf1" />


## What didn't got well

## What did go well
1. 👍 Memory of the boilerplate with `header`, `nav`, `article`, `section`+`id` is still fresh so was able to write the refreshed boilerplate upfront with placeholder content.

----

# Suggestions
1. Again maybe it's just my personal preference, but the approach of trying to write the HTML without referring to the instrutions first enhance your learnining by focusing on things you missed/got wrong/forgot about.

[Ends 16:15 28 Sep 2025]
