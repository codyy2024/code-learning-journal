# Day 52: Lab - Build a Multimedia Player

## Key topics covered
- [x] `audio `, `video`
- [x] `aria-label`

I've forgotten about video and audieo elements, and what `aria-label` is used for so...

What I did following the instructions
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Multimedia Player</title>
    </head>
    <body>
        <main>
            <h1>Multimedia Player</h1>
            <section id="audio">
                <h2>Now Playing: Sailing Away</h2>
                <audio controls aria-label="song sailing away is playing">
                    <source src="https://cdn.freecodecamp.org/curriculum/js-music-player/sailing-away.mp3" type="mp3">
                </audio>
            </section>
            <section id="video">
                <h2>What is a map method and how does it work?</h2>
                <video
                controls
                width="560"
                >
                    <source src="https://cdn.freecodecamp.org/curriculum/labs/what-is-the-map-method-and-how-does-it-work.mp4" type="mp4">
                    <track src="test.ytt" kind="captions" srclang="en" label="English">
                </video>
            </section>    
            <section id="transcript">
                <h2>Transcript</h2>
                <p>What is a map method and how does it work? The map method is a powerful and widely used function in JavaScript that operates on arrays. It's designed to create a new array by applying a given function to each element of the original array. This method does not modify the original array, but instead returns the new array containing the results of the function applied to each element.</p>
            </section>
        </main>
    </body>
</html>
```
It passsed, but I'm still not quite sure why mine didn't render the audio and video

## What didn't go well
Everything 😢

## What did go well
Nothing 😢

## Suggestions
Only to myself - but I do't know what to say!

[Ends 21:02 24 Oct 2025]



