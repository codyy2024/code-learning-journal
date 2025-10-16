# Day 44: Workshop - Build a Conference Schedule Table

What I wrote in VS Code:
```
<!-- Build a Conference Schedule Table -->
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Build a Conference Schedule Table</title>
    </head>
    <body>
        <main>
            <header>
                <h1>Tech Conference 2025 Schedule</h1>
            </header>
            <table>
                <caption>Schedule by Track and Time</caption>
                <thead>
                    <tr>
                        <th scope="col">Time</th>
                        <th scope="col" colspan="2">Track A</th>
                        <th scope="col" colspan="2">Track B</th>
                        <th scope="col" colspan="2">Track C</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <th scope="row">9:00 AM</th>
                        <td scope="row" colspan="2">Keynote: Tech Future</td>
                        <td scope="row" colspan="2">Intro to Web Dev</td>
                        <td scope="row" colspan="2">UX for All</td>
                    </tr>
                    <tr>
                        <th scope="row">10:00 AM</th>
                        <td scope="row" colspan="2">Accessibility Deep Dive</td>
                        <td scope="row" colspan="2">CSS for Beginners</td>
                        <td scope="row" colspan="2">Inclusive Design Principles</td>
                    </tr>
                    <tr>
                        <th scope="row">11:00 AM</th>
                        <td scope="row" colspan="2">Break</td>
                    </tr>
                    <tr>
                        <th scope="row">11:30 AM</th>
                        <td scope="row" colspan="2">AR/VR in Education</td>
                        <td scope="row" colspan="2">JavaScript Fundamentals</td>
                        <td scope="row" colspan="2">Design Systems at Scale</td>
                    </tr>
                    <tr>
                        <th scope="row">12:30 PM</th>
                        <td scope="row" colspan="2">Lunch Break</td>
                    </tr>
                    <tr>
                        <th scope="row">2:00 PM</th>
                        <td scope="row" colspan="2">Voice UI Workshop</td>
                        <td scope="row" colspan="2">Git & GitHub Essentials</td>
                        <td scope="row" colspan="2">Color & Contrast in UI</td>
                    </tr>
                </tbody>
            </table>
        </main>
    </body>
</html>
```

Renders okay (though when I copied and paste, each and every data cell is `th` so they were all bold!)

Followed the instructions and it was exactly the same except the `colspan` for the two Break rows were `colspan="3"` instead of 2.

So all good!

[Ends 21:11 15 Oct 2025]
