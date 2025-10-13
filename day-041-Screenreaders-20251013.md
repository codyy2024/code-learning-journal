# Day 41: Theory - Importance Of Accessibility and Good HTML Structure

## Key topics covered:
- [x] What are screen readers (and what screen reader are not)
- [ ] Who use screen readers
- [ ] Screen reader friendiless and challenges
- [ ] What Are Large Text or Braille Keyboards, and Who Uses Them
- [ ] What Are Alternative Pointing Devices
- [ ] Screen magnifiers
- [ ] Voice Recognition Software
- [ ] Accessibility auditing tools
- [ ] How Does Proper Heading Level Structure Affect Accessibility?

## 1. What are screen readers
Screen readers are assistive technology programs that help blind and visually impaired people use computers and mobile devices, to acess education, work opportunities, and social media

They are **not** simply just text-to-speech devices. Screen readers can do more than that, to name a few below:
- text-to-speech
- text to braille
- navigation aids
- web browsing assistance

## 2. Who uses screen readers
- The blind and visually impaired
- Dyslexic individuals
- People with cognitive disabilities

## 3. All the popular OSs have screen readers built in
- macOS and iOS: VoiceOver
- Windows: Narrator. Also available:
  - NonVisual Desktop Access (NVDA): free
  - Job Access With Speech (JAWS): paid
- Linux: ***Orca*** for the desktop environment and ***Speakup*** for the Linux terminal
- Android: TalkBack, Ella or Select to Speak

## 4. Challenges for screenreader users
One major chanllenge: many software developers don't design their products with screen-reader friendliness and accessibility in mind.

[Ends 09:15 13 Oct 2025]

====

[Starts 19:40 13 Oct 2025]

## 5. Large Text or Braille Keyboards
### 5.1 Large print keyboard: helpful for people with low vision
- MaxiAids: has yellow keys with black, big, and bold letters, numbers, and symbols on them. 
- black large print keyboard with white print on the keys (backlit)

### 5.2 Braille keyboard: for people with more severe vision disabilities, including people who are blind.

Some keyboards combine both approaches - helpful for people with visual disabilities and for people who are learning braille.

## 6. What Are Alternative Pointing Devices Such as Trackballs, Joysticks, and Touchpads Used For?
Alternative pointing devices are input devices that make good alternatives to the traditional mouse.

| Type of alternative pointing device | What it is | What it is good for | Who it is for |
| --- | ---- | ---- | --- | 
| Trackball | A stationary pointing device that consists of a large, movable ball within a socket. Also includes additional buttons for clicking and performing other functions. | Users manipulate the ball directly with their fingers, thumb, or palm to move the cursor on the screen. Therefore reduce the physical movement the user needs for navigation | Ideal for users with mobility issues |
| Joystick | A pointing device primarily designed for games and certain industrial applications like machinery control. | Accommodate larger and more deliberate movements; also reduce the strain and pain that comes with repetitive movements | Beneficial for individuals with tremors and unsteady hands, or individuals with arthritis and carpal tunnel syndrome. |
| Touchpad |  A flat, touch-sensitive device built into laptops and some keyboards. | Significantly enhance navigation by supporting multi-touch gestures like pinch-to-zoom, two-finger scrolling, tap-to-click, and three-finger swipes. | Ideal for individuals with low arm or hand movement, or people with arthritis and joint pain |

## 7. Screen magnifiers
Screen magnifiers work by enlarging texts, graphics, and other elements on a computer or mobile device screen. 

Software developers need to make their digital products accessible to people with low vision. Some considerations include:
- Using scalable fonts so the user can resize the page without the layout breaking.
- Ensuring the user interface adapts to different screen sizes through responsive design.
- Using high-contrast color schemes and customizable colors.
- Implementing a non-sticky and tiny navbar so users can still see content when using magnifiers.
- Using regular HTML text instead of images of text.
- Providing feedback directly next to the element that triggers it, and more.

Screen magnifiers built in mainstream OSs: Zoom, Manigication, Magnifier

## 8. Voice recognition

## 9. Common Accessibility Auditing Tools
1. Google Lighthouse - in Chrome or online
   - in Chrome: can check both live websites and locally developed ones
   - [web version](pagespeed.web.dev): more reliable but can only check live websites
2. WAVE: a Chrome extension
3. IBM Equal Accessibility Checker

They typically will only find about a third of all possible accessibility issues. Manual testing, preferably by people with disabilities, will always be required to ensure that your content is as accessible as possible.

## 10. How Does Proper Heading Level Structure Affect Accessibility?
Headings, ranging from h1 to h6, create a navigational structure for screen reader users, allowing users to jump directly to the sections they need.

Here are some key practices to follow to use headings properly:
- Use headings in a hierarchy that reflects clear organization. For example, the page title should be an  `h1`, major sections should be introduced with `h2` headings, subsections with `h3` , and so on, down to h6.
- Don't skip from `h1` to `h3`, or from `h2` to `h`, and so on.
- Use clear and descriptive text that summarizes the content that follows each heading.
- Don't use a heading in isolation – some content must follow the heading.
- Use appropriate headings where necessary instead of formatting text to look like headings.
- Each page should have a single `h1` element representing the main topic or title.

A basic markup that represents how you should use headings on a page:
```
<!-- Page title -->
<h1>What is HTML</h1>

<!-- First section -->
<section>
  <h2>Introduction to HTML</h2>
  <p>
    HTML stands for HyperText Markup Language. It is the standard language for
    creating web pages.
  </p>
</section>
<!-- Second section -->
<section>
  <h2>History of HTML</h2>
  <p>HTML began to take shape in the early 90s</p>
  <h3>Origins</h3>
  <p>
    HTML was created by Tim Berners-Lee in 1991. It has evolved significantly
    over the years.
  </p>
</section>
```


