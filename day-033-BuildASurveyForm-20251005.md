# Day 33: Lab - Build A Survey Form

## Key topics covered:
- [x] review `form`
- [x] different `input` elements
- [x] the `required` attribute
- [x] more

What I wrote in VS Code:
```
<!DOCCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Survey Form</title>
    </head>#
    <body>
        <header>
            <h1>FreeCodeCamp Survey Form</h1>
            <p>Thank you for taking the time to help us improve the platform</p>
        </header>
        <main>
            <form method="get" action="">
                <section id="personal-information">
                    <p>
                        <label for="name">Name</label>
                        <input type="text" id="name" placeholder="Enter your name" required />
                        <br />
                        <label for="email">Email</label>
                        <input type="email" id="email" placeholder="Enter your Email" required />
                        <br />
                        <label for="age">Age (optional)</label>
                        <input type="number" id="age" placeholder="Age" min="3" max="100" />
                    </p>
                    <p>
                        <label for="role">Which option best describes your current role?</label>
                    </p>
                    <p>
                        <select id="role" name="role">
                            <option value="select-current-role" selected deactivated>Select current role</option> <!--1st thing I'm not sure of - doesn't seem like the "deactivated" (greyed out) function is right -->
                            <option value="student">Student</option>
                            <option value="full-time-job">Full Time Job</option>
                            <option value="full-time-learner">Full Time Learner</option>
                            <option value="prefer-not-to-say">Prefer not to say</option>
                        </select>
                    </p>
                </section>
                <section id="freecodecamp-q">
                    <p>Would you reccommend freeCodeCamp to a friend?</p><!-- 2nd thing I'm not super sure of - should this be <label> which has id or a <p> which doesn't have id -->
                    <p>
                        <input type="radio" id="definitely" name="definitely" value="definitely" checked />
                        <label for="definitely">Definitely</label>
                        <input type="radio" id="maybe" name="maybe" value="maybe" />
                        <label for="maybe">Maybe</label>
                        <input type="radio" id="not-sure" name="not-sure" value="not-sure" />
                        <label for="not-sure">Not sure</label>
                    </p>
                    <p>What is your favorite feature of freeCodeCamp?</p>
                    <p>
                        <select id="fav-of-freecodecamp" name="fav-of-freecodecamp">
                            <option value="select-an-option" selected deactivated>Select an option</option>
                            <option value="challenges">Challenges</option>
                            <option value="projects">Projects</option>
                            <option value="community">Community</option>
                            <option value="open-source">Open Source</option>
                        </select>
                    </p>
                    <p>
                        What would you like to see improved? (Check all that apply)
                    </p>
                    <p>
                        <input type="checkbox" id="front-end-projects" name="improve-feedback" value="front-end-projects" />
                        <label for="front-end-projects">Front-end Projects</label>
                        <input type="checkbox" id="back-end-projects" name="improve-feedback" value="back-end-projects" />
                        <label for="back-end-projects">Back-end Projects</label>
                        <input type="checkbox" id="data-visualisation" name="improve-feedback" value="data-visualisation" />
                        <label for="data-visualisation">Data Visualisation</label>
                        <input type="checkbox" id="challenges" name="improve-feedback" value="challenges" />
                        <label for="challenges">Challenges</label>
                        <input type="checkbox" id="open-source-community" name="improve-feedback" value="open-source-community" />
                        <label for="open-source-community">Open Source Communitu</label>
                        <input type="checkbox" id="gitter-help-rooms" name="improve-feedback" value="gitter-help-rooms" />
                        <label for="gitter-help-rooms">Gitter help rooms</label>
                        <input type="checkbox" id="videos" name="improve-feedback" value="videos" />
                        <label for="videos">Videos</label>
                        <input type="checkbox" id="city-meetups" name="improve-feedback" value="city-meetups" />
                        <label for="city-meetups">City Meetups</label>
                        <input type="checkbox" id="wiki" name="improve-feedback" value="wiki" />
                        <label for="wiki">Wiki</label>
                        <input type="checkbox" id="forum" name="improve-feedback" value="forum" />
                        <label for="forum">Forum</label>
                        <input type="checkbox" id="additional-courses" name="improve-feedback" value="additional-courses" />
                        <label for="additional-courses">Additional Courses</label>
                    </p>
                    <p>Any comments or suggestions?</p>
                    <p>
                        <textarea id="comments" placeholder="Enter your comment here..." cols="20" rows="2"></textarea>
                        <br />
                        <button type="submit">Submit</button>
                    </p>
                </section>
            </form>
        </main>
    </body>
</html>
```

A few things noticed after reading the instrutions:
1. it asks to add `id` to `form`, `label`, `h1` and the `p` under `h1` which was not covered in the previous lectures
2. it asks to add `description`, but where does it go?

Even though i passed it, 
- i still don't know what these ids are used for?
- i put the `description` just in the `header` after `p` but not sure what these are used for?
- some of the `label`s probs are not needed/need to be `p` - but it still passed so no idea i was wrong/right as it only seems to focus on the intruction bullet points and if all of those are right, it gives me a pass.

End result after amending following the instructions:   
```
<!DOCCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Survey Form</title>
    </head>#
    <body>
        <header>
            <h1 id="title">FreeCodeCamp Survey Form</h1>
            <p id="description">Thank you for taking the time to help us improve the platform</p>
            <title>FreeCodeCamp Survey Form</title>
            <description>This is the FreeCodeCamp Survey Form description</description>
        </header>
        <main>
            <form method="get" action="" id="survey-form">
                <section id="personal-information">
                    <p>
                        <label for="name" id="name-label">Name</label>
                        <input type="text" id="name" placeholder="Enter your name" required />
                        <br />
                        <label for="email" id="email-label">Email</label>
                        <input type="email" id="email" placeholder="Enter your Email" required />
                        <br />
                        <label for="number" id="number-label">Age (optional)</label>
                        <input type="number" id="number" placeholder="Age" min="3" max="100" />
                    </p>
                    <p>
                        <label for="role">Which option best describes your current role?</label>
                    </p>
                    <p>
                        <select id="dropdown" name="role">
                            <option value="select-current-role" selected disabled>Select current role</option> <!--1st thing I'm not sure of - doesn't seem like the "deactivated" (greyed out) function is right -->
                            <option value="student">Student</option>
                            <option value="full-time-job">Full Time Job</option>
                            <option value="full-time-learner">Full Time Learner</option>
                            <option value="prefer-not-to-say">Prefer not to say</option>
                        </select>
                    </p>
                </section>
                <section id="freecodecamp-q">
                    <p>Would you reccommend freeCodeCamp to a friend?</p><!-- 2nd thing I'm not super sure of - should this be <label> which has id or a <p> which doesn't have id -->
                    <p>
                        <input type="radio" id="definitely" name="reccommend" value="definitely" checked />
                        <label for="definitely">Definitely</label>
                        <input type="radio" id="maybe" name="reccommend" value="maybe" />
                        <label for="maybe">Maybe</label>
                        <input type="radio" id="not-sure" name="reccommend" value="not-sure" />
                        <label for="not-sure">Not sure</label>
                    </p>
                    <p>What is your favorite feature of freeCodeCamp?</p>
                    <p>
                        <select id="dropdown" name="fav-of-freecodecamp">
                            <option value="select-an-option" selected disabled>Select an option</option>
                            <option value="challenges">Challenges</option>
                            <option value="projects">Projects</option>
                            <option value="community">Community</option>
                            <option value="open-source">Open Source</option>
                        </select>
                    </p>
                    <p>
                        What would you like to see improved? (Check all that apply)
                    </p>
                    <p>
                        <input type="checkbox" id="front-end-projects" name="improve-feedback" value="front-end-projects" />
                        <label for="front-end-projects">Front-end Projects</label>
                        <input type="checkbox" id="back-end-projects" name="improve-feedback" value="back-end-projects" />
                        <label for="back-end-projects">Back-end Projects</label>
                        <input type="checkbox" id="data-visualisation" name="improve-feedback" value="data-visualisation" />
                        <label for="data-visualisation">Data Visualisation</label>
                        <input type="checkbox" id="challenges" name="improve-feedback" value="challenges" />
                        <label for="challenges">Challenges</label>
                        <input type="checkbox" id="open-source-community" name="improve-feedback" value="open-source-community" />
                        <label for="open-source-community">Open Source Communitu</label>
                        <input type="checkbox" id="gitter-help-rooms" name="improve-feedback" value="gitter-help-rooms" />
                        <label for="gitter-help-rooms">Gitter help rooms</label>
                        <input type="checkbox" id="videos" name="improve-feedback" value="videos" />
                        <label for="videos">Videos</label>
                        <input type="checkbox" id="city-meetups" name="improve-feedback" value="city-meetups" />
                        <label for="city-meetups">City Meetups</label>
                        <input type="checkbox" id="wiki" name="improve-feedback" value="wiki" />
                        <label for="wiki">Wiki</label>
                        <input type="checkbox" id="forum" name="improve-feedback" value="forum" />
                        <label for="forum">Forum</label>
                        <input type="checkbox" id="additional-courses" name="improve-feedback" value="additional-courses" />
                        <label for="additional-courses">Additional Courses</label>
                    </p>
                    <p>Any comments or suggestions?</p>
                    <p>
                        <textarea id="comments" placeholder="Enter your comment here..." cols="20" rows="2"></textarea>
                        <br />
                        <button type="submit" id="submit">Submit</button>
                    </p>
                </section>
            </form>
        </main>
    </body>
</html>
```

## What didn't go well
1. Almost forgot about the `select` element - though remembered most of the `option` element within it (except the "deactivated" function - at least I realised that the "Select an option" needs to be deactivated!)
2. Used to the `fieldset` element from Day 32, but not too sure about when we're not using that - I used `p` and `br` to achieve the same results but not sure if it's supposed to be like that

## What did go well
1. Boilerplate is still online
2. Though forgot some, I remember most of the stuff of the previous couple of days, which might be due to the fact I did a few rounds of revisits

## Suggestions
1. Some of the wording of the instrutions are not clear
   Examples:
   - i think i know what "descedents" mean, but this terminology was never used so far until now
   - what does it mean by "#name-label"?
   - what do you mean by "Every radio button **group**"?
   
