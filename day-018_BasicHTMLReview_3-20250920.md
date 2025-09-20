# Day 18: Basic HTML Review Part 3

(Continued from Day 17)

## Boilerplate and Encoding
- boilerplate
  - `head` section contains important meta data which is behind-the-scenes information needed for browsers and search engines.
- SEO and social sharing (using my [published site](https://codyy2024.github.io/code-learning-journal/) as a real learning example)
  - `description` and  `content`: set a short description of the web page to impact SEO
      ```
      <meta name="descrition" content="My journey from a complete coding newbie to completing the Full Stack Developer Curriculum on freeCodeCamp">
      ```
  
  - open graph tags (og:xx): a protocol enables you to control how your website's content appears across various social media platforms
    ```
    <meta property="og:title" content="code-learning-journal">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://codyy2024.github.io/code-learning-journal/">
    ```

  ## Media Elements and Optimization
  - Replaced elements: whos content is determinded by external source (`img`, `iframe`, `audio`, `video`, `embed`, `a`(?) etv.)
    > Same old questions:
      1. what is the conception of frame in the first place?
      2. what is the difference of `src` versus `href`?
    > New questions: what is cross origin and how is it used?
  - Optimising media: the size, the format, and the compression
  - Image formats: a more optimized format, like WEBP or AVIF
  - Image license: public, CC0 license, full licence
  - SVGs (Scalable Vector Graphics): can be scaled without impacting the quality
  - Multimedia integration
    - `audieo`: supports .mp3, .wav and .ogg; `video`: supports .mp4, .gg and .webm
      - `controls` attribute (boolean): show audio player (if not added, then means == false i.e. audio player not showing)
      - `loop` attribute (boolean)
      - `muted` attribute (boolean)
      - `source` element: used inside the `audio` element and the browser will select the first source that it understands.
        ```
        <audio controls>
          <source src="audio.ogg" type="audio/ogg" />
          <source src="audio.wav" type="audio/wav" />
          <source src="audio.mp3" type="audio/mpeg" />
        </audio>
        ```
        **Q**: believe this `source` element can be used for `video` too?
      - `poster` attribute: unique to video element - display an image while video is downloading

## Taget Attribute types
- `_self`, `_blank`, `_parent`, `_top`

## Absolute Paths vs. Relative Paths
- Absolute paths: a complete link to a resource (which also includes the protocol - `http`, `https` and `file`) or domain name if resource is on the web.
- Relative:

## Link status
`:link`, `:visited`, `hover`, `focus`, `active`

Basic HTML Review DONE!

---

## What didn't go well
1. I'd forgotten some of the content already. In hindsight, I think we could be benefit with more hands on practice with each after a few lessons, as opposed to simple multiple choice questions.
2. Some of the one-line definition of an element was new and not said that way in the previous/original lessons. So would benefit if it could be consistent and/or those clear definition is broufht forward.
