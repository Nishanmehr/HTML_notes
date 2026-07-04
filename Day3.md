# 📘 HTML Day 3 - Part 1
# Class, ID, Internal Navigation & Semantic HTML

---

# 📌 Overview

In this part, we will learn:

- class
- id
- Difference between class and id
- Internal Navigation
- Semantic HTML
- Header
- Nav
- Main
- Section
- Article
- Aside
- Footer

---

# 1. class Attribute

## Definition

The `class` attribute is used to group multiple HTML elements together.

Multiple elements can have the same class name.

It is mainly used for CSS styling and JavaScript.

---

## Syntax

```html
<h1 class="logo">Nishant Mehra</h1>

<p class="logo">
Hello
</p>
```

Both elements belong to the same class.

---

## Example

```html
<h2 class="heading">
About
</h2>

<h2 class="heading">
Projects
</h2>

<h2 class="heading">
Contact
</h2>
```

All headings share the same class.

---

## Why use class?

Suppose you have

- 10 buttons

Instead of styling them one by one,

give all of them

```html
class="btn"
```

Now CSS can style all buttons together.

---

## Rules

✅ Can be reused

✅ One element can have multiple classes

Example

```html
<div class="box active">
```

---

# 2. id Attribute

## Definition

The `id` attribute uniquely identifies an HTML element.

Only one element should have a particular id.

---

## Syntax

```html
<h2 id="about">
About
</h2>
```

---

## Example

```html
<h2 id="contact">
Contact
</h2>
```

---

## Rules

✅ Must be unique

❌ Never repeat the same id.

Wrong

```html
<p id="name"></p>

<p id="name"></p>
```

Correct

```html
<p id="firstName"></p>

<p id="lastName"></p>
```

---

# Difference between Class and ID

| Class | ID |
|--------|----|
| Used for multiple elements | Used for one element |
| Can repeat | Cannot repeat |
| CSS selector: .class | CSS selector: #id |

---

# 3. Internal Navigation

Internal navigation means jumping to another section of the same webpage.

---

## Syntax

### Step 1

Create a link.

```html
<a href="#contact">
Contact
</a>
```

---

### Step 2

Give that section an id.

```html
<h2 id="contact">

Contact

</h2>
```

---

## Working

Click

```html
<a href="#contact">
```

↓

Browser searches

```html
id="contact"
```

↓

Automatically scrolls there.

---

## Example

```html
<nav>

<a href="#about">

About

</a>

<a href="#projects">

Projects

</a>

<a href="#contact">

Contact

</a>

</nav>

<section>

<h2 id="about">

About

</h2>

</section>

<section>

<h2 id="projects">

Projects

</h2>

</section>

<footer>

<h2 id="contact">

Contact

</h2>

</footer>
```

---

# 4. Semantic HTML

## Definition

Semantic tags describe the meaning of the content.

Instead of

```html
<div>
```

we use

```html
<header>

<nav>

<main>

<footer>
```

This improves

- readability
- SEO
- accessibility

---

# Semantic Layout

```

<header>

<nav>

<main>

<section>

<article>

<aside>

<footer>

```

---

# 5. Header

Represents introductory content.

Usually contains

- Logo
- Website name
- Navigation

Example

```html
<header>

<h1>

Nishant Mehra

</h1>

</header>
```

---

# 6. Nav

Represents navigation links.

Example

```html
<nav>

<a href="#about">

About

</a>

<a href="#projects">

Projects

</a>

</nav>
```

---

# 7. Main

Represents the main content of the page.

There should usually be only one `<main>` element.

Example

```html
<main>

...

</main>
```

---

# 8. Section

Groups related content.

Example

```html
<section>

<h2>

Skills

</h2>

<p>

HTML CSS JavaScript

</p>

</section>
```

---

# 9. Article

Represents independent content.

Examples

- Blog post
- News article
- Product review

Example

```html
<article>

<h2>

HTML Tutorial

</h2>

<p>

Learn HTML...

</p>

</article>
```

---

# 10. Aside

Contains side content.

Examples

- Advertisements
- Sidebar
- Related posts

Example

```html
<aside>

Related Articles

</aside>
```

---

# 11. Footer

Represents the bottom section.

Usually contains

- Copyright
- Contact
- Social links

Example

```html
<footer>

<p>

Copyright © 2026

</p>

</footer>
```

---

# Complete Structure

```html
<body>

<header>

</header>

<nav>

</nav>

<main>

<section>

</section>

<section>

</section>

</main>

<footer>

</footer>

</body>
```

---

# Best Practices

✅ Use only one `<main>`

✅ Keep navigation inside `<nav>`

✅ Group similar content inside `<section>`

✅ Footer should contain contact/copyright.

✅ Use meaningful ids.

---

# Common Mistakes

❌ Repeating ids

❌ Using only div everywhere

❌ Forgetting closing tags

❌ Placing footer inside header

❌ Multiple main tags

---

# Interview Questions

1. What is the difference between class and id?

2. Can multiple elements have the same id?

3. Why do we use semantic HTML?

4. Difference between div and section?

5. Difference between section and article?

6. Difference between head and header?

7. Difference between main and section?

8. What is internal navigation?

9. Why is id used with href?

10. Why should ids be unique?

# 📘 HTML Day 3 - Part 2
# Multimedia in HTML

---

# 📌 Overview

In this part, we will learn:

- Image
- img Tag
- src Attribute
- alt Attribute
- width
- height
- Relative Path
- Absolute Path
- figure
- figcaption
- audio
- video
- source
- controls
- autoplay
- muted
- loop
- poster
- picture

---

# 1. Images in HTML

## Definition

Images make a webpage more attractive and informative.

HTML uses the `<img>` tag to display images.

---

## Syntax

```html
<img src="profile.jpg" alt="Profile Picture">
```

---

## img Tag

The `<img>` tag is a self-closing tag.

```html
<img src="image.jpg" alt="Image">
```

---

# 2. src Attribute

## Definition

The `src` attribute tells the browser where the image is located.

Example

```html
<img src="photo.jpg">
```

---

# 3. alt Attribute

## Definition

Alternative text shown when an image cannot be loaded.

It is also used by screen readers.

Example

```html
<img
src="profile.jpg"
alt="Nishant Mehra">
```

---

## Why is alt important?

✅ Accessibility

✅ SEO

✅ Broken image description

---

# 4. width Attribute

Controls image width.

Example

```html
<img
src="profile.jpg"
width="200">
```

---

# 5. height Attribute

Controls image height.

Example

```html
<img
src="profile.jpg"
height="200">
```

---

# Best Practice

Always specify both width and height.

```html
<img
src="profile.jpg"
alt="Profile"
width="200"
height="200">
```

---

# 6. Relative Path

Points to files inside your project.

Example

```html
<img src="images/profile.jpg">
```

Folder Structure

```
Project
│
├── index.html
│
└── images
      └── profile.jpg
```

---

# 7. Absolute Path

Uses a complete URL.

```html
<img src="https://example.com/profile.jpg">
```

---

# Relative vs Absolute

| Relative Path | Absolute Path |
|---------------|---------------|
| Local file | Internet URL |
| Faster | Requires Internet |
| Used most | Used for online images |

---

# 8. figure Tag

Represents self-contained content.

Mostly used for

- Images
- Charts
- Diagrams

Example

```html
<figure>

<img
src="profile.jpg"
alt="Profile">

</figure>
```

---

# 9. figcaption

Provides a caption for the figure.

Example

```html
<figure>

<img
src="profile.jpg"
alt="Profile">

<figcaption>

My Profile Picture

</figcaption>

</figure>
```

---

# Why use figure?

It groups an image with its description.

---

# 10. Audio

HTML5 introduced the `<audio>` tag.

Example

```html
<audio controls>

<source
src="song.mp3"
type="audio/mpeg">

</audio>
```

---

# controls

Shows play, pause, volume, and progress controls.

```html
<audio controls>
```

---

# autoplay

Automatically starts audio.

```html
<audio autoplay>
```

⚠ Most browsers block autoplay unless muted.

---

# muted

Starts audio in mute mode.

```html
<audio muted>
```

---

# loop

Repeats audio forever.

```html
<audio loop>
```

---

# source Tag

Provides media files.

Example

```html
<source
src="song.mp3"
type="audio/mpeg">
```

---

# Multiple Sources

```html
<audio controls>

<source
src="song.mp3"
type="audio/mpeg">

<source
src="song.ogg"
type="audio/ogg">

</audio>
```

Browser chooses the supported format.

---

# Browser Fallback

```html
<audio controls>

<source
src="song.mp3"
type="audio/mpeg">

Your browser does not support audio.

</audio>
```

---

# 11. Video

HTML5 video player.

Example

```html
<video controls>

<source
src="video.mp4"
type="video/mp4">

</video>
```

---

# width

```html
<video
width="400">
```

---

# height

```html
<video
height="250">
```

---

# controls

Shows play and pause buttons.

```html
controls
```

---

# autoplay

Starts video automatically.

```html
autoplay
```

---

# muted

Required if autoplay is used.

```html
muted
```

---

# loop

Repeats video.

```html
loop
```

---

# poster

Displays an image before the video starts.

Example

```html
<video
controls
poster="thumbnail.jpg">
```

---

# Complete Example

```html
<video
width="400"
controls
poster="thumbnail.jpg">

<source
src="intro.mp4"
type="video/mp4">

Your browser does not support video.

</video>
```

---

# 12. Picture Tag

Used for responsive images.

Example

```html
<picture>

<source
media="(max-width:600px)"
srcset="mobile.jpg">

<source
media="(min-width:601px)"
srcset="desktop.jpg">

<img
src="desktop.jpg"
alt="Profile">

</picture>
```

---

# Why use picture?

Different images can be shown on

- Mobile
- Tablet
- Desktop

---

# img vs picture

| img | picture |
|------|----------|
| One image | Multiple images |
| Simple | Responsive |

---

# Best Practices

✅ Always provide alt.

✅ Specify width and height.

✅ Use figure + figcaption.

✅ Use controls for audio/video.

✅ Use poster for videos.

✅ Use multiple source tags.

✅ Add fallback text.

---

# Common Mistakes

❌ Forgetting alt.

❌ Writing

```html
<audio control>
```

Correct

```html
<audio controls>
```

---

❌ Forgetting source tag.

Wrong

```html
<audio>

</audio>
```

---

Correct

```html
<audio controls>

<source
src="song.mp3"
type="audio/mpeg">

</audio>
```

---

❌ Forgetting poster.

---

❌ Using huge images.

Always optimize images.

---

# Interview Questions

1. What is the img tag?

2. Difference between src and alt?

3. Why is alt important?

4. Difference between relative and absolute path?

5. What is figure?

6. Why use figcaption?

7. Difference between audio and source?

8. Why use controls?

9. Why do browsers block autoplay?

10. What is poster?

11. Difference between img and picture?

12. Why use picture?

13. Why use multiple source tags?

14. Difference between width and height?

15. What is fallback text?

---
# 📘 HTML Day 3 - Part 3
# iframe, HTML Entities, Meta Tags, Accessibility & Best Practices

---

# 📌 Overview

In this part, we will learn:

- iframe
- HTML Entities
- Meta Tags
- Accessibility
- HTML Best Practices
- HTML Interview Tips

---

# 1. iframe

## Definition

The `<iframe>` (Inline Frame) tag is used to embed another webpage inside your current webpage.

Common uses:

- YouTube Videos
- Google Maps
- PDF Viewer
- External Webpages

---

## Syntax

```html
<iframe
src="https://example.com">
</iframe>
```

---

## Example - YouTube Video

```html
<iframe
width="560"
height="315"
src="https://www.youtube.com/embed/VIDEO_ID"
title="HTML Tutorial"
allowfullscreen>
</iframe>
```

---

## Example - Google Maps

```html
<iframe
src="https://www.google.com/maps/embed?..."
width="600"
height="450"
title="Google Map">
</iframe>
```

---

## Important Attributes

### src

Specifies the URL of the webpage or content.

```html
src=""
```

---

### width

Sets iframe width.

```html
width="600"
```

---

### height

Sets iframe height.

```html
height="400"
```

---

### title

Provides a description for accessibility.

```html
title="Company Location"
```

---

### allowfullscreen

Allows fullscreen mode.

```html
allowfullscreen
```

---

## Interview Question

### Can every website be embedded inside an iframe?

❌ No.

Many websites block embedding using security headers such as:

- X-Frame-Options
- Content-Security-Policy

---

# 2. HTML Entities

## Definition

HTML Entities display reserved characters or special symbols.

---

## Less Than

```html
&lt;
```

Output

```
<
```

---

## Greater Than

```html
&gt;
```

Output

```
>
```

---

## Ampersand

```html
&amp;
```

Output

```
&
```

---

## Copyright

```html
&copy;
```

Output

```
©
```

---

## Registered

```html
&reg;
```

Output

```
®
```

---

## Trademark

```html
&trade;
```

Output

```
™
```

---

## Non-Breaking Space

```html
&nbsp;
```

Creates a space that doesn't collapse.

Example

```html
Hello&nbsp;&nbsp;&nbsp;World
```

---

## Rupee Symbol

```html
&#8377;
```

Output

```
₹
```

---

## Euro Symbol

```html
&euro;
```

Output

```
€
```

---

# 3. Meta Tags

Meta tags provide information **about the webpage**.

They are placed inside the `<head>` section.

---

## Charset

```html
<meta charset="UTF-8">
```

Supports almost all languages.

---

## Viewport

```html
<meta
name="viewport"
content="width=device-width, initial-scale=1.0">
```

Makes websites responsive on mobile devices.

---

## Description

```html
<meta
name="description"
content="Portfolio Website">
```

Used by search engines.

---

## Keywords

```html
<meta
name="keywords"
content="HTML,CSS,Portfolio">
```

Provides search keywords.

---

## Author

```html
<meta
name="author"
content="Nishant Mehra">
```

Specifies the author.

---

# Why Use Meta Tags?

✅ SEO

✅ Mobile Responsiveness

✅ Browser Information

✅ Search Engine Results

---

# 4. Accessibility

## Definition

Accessibility means making websites usable for everyone, including users with disabilities.

---

## Always Use alt

Good

```html
<img
src="profile.jpg"
alt="Nishant Mehra">
```

Bad

```html
<img
src="profile.jpg">
```

---

## Always Use Labels

Good

```html
<label for="email">

Email

</label>

<input
id="email">
```

---

## Use Semantic HTML

Good

```html
<header>

<nav>

<main>

<footer>
```

Instead of only using:

```html
<div>
```

---

## Buttons

Wrong

```html
<div>

Submit

</div>
```

Correct

```html
<button>

Submit

</button>
```

---

## iframe

Always provide a title.

```html
<iframe
title="Google Map">
```

---

# 5. HTML Best Practices

## Indentation

Good

```html
<div>

    <p>Hello</p>

</div>
```

---

## Meaningful Names

Bad

```html
id="a"
```

Good

```html
id="employeeName"
```

---

## Close Every Tag

Wrong

```html
<p>

Hello
```

Correct

```html
<p>

Hello

</p>
```

---

## Use Lowercase Tags

Good

```html
<body>

<p>
```

Avoid

```html
<BODY>

<P>
```

---

## Use Semantic Elements

Prefer

```html
<header>

<nav>

<section>

<footer>
```

Instead of

```html
<div>
```

---

## Use Unique IDs

Wrong

```html
<input id="name">

<input id="name">
```

Correct

```html
<input id="firstName">

<input id="lastName">
```

---

## Keep Buttons Inside Forms

Correct

```html
<form>

...

<button type="submit">

Submit

</button>

</form>
```

---

## Optimize Images

✔ Use compressed images.

✔ Add width and height.

✔ Always include alt.

---

# Common Mistakes

❌ Missing alt attribute

❌ Duplicate IDs

❌ Using div everywhere

❌ Buttons outside forms

❌ Missing iframe title

❌ Using huge image files

❌ Forgetting viewport meta tag

---

# HTML Interview Questions

## Basics

1. What is HTML?
2. What is HTML5?
3. Difference between HTML and HTML5?

---

## Attributes

4. Difference between id and class?
5. Difference between src and href?
6. Difference between readonly and disabled?
7. Difference between GET and POST?

---

## Tables

8. What is colspan?
9. What is rowspan?
10. Difference between thead, tbody and tfoot?

---

## Forms

11. Why is the name attribute important?
12. Difference between radio and checkbox?
13. Difference between placeholder and value?
14. What is pattern?
15. What is required?

---

## Semantic HTML

16. Difference between div and span?
17. Difference between section and article?
18. Difference between head and header?
19. Difference between nav and header?
20. Why use semantic HTML?

---

## Multimedia

21. Difference between img and picture?
22. What is figure?
23. Why use figcaption?
24. What is poster?
25. Why use source?

---

## Advanced

26. What is iframe?
27. What are HTML entities?
28. Why use meta tags?
29. What is accessibility?
30. Why is alt important?

---

# HTML Revision Checklist

## Structure

- [x] HTML Boilerplate
- [x] Head
- [x] Body

---

## Text

- [x] Headings
- [x] Paragraphs
- [x] Formatting Tags

---

## Lists

- [x] ul
- [x] ol
- [x] li

---

## Links

- [x] a
- [x] href
- [x] Internal Navigation

---

## Images

- [x] img
- [x] alt
- [x] figure
- [x] figcaption

---

## Tables

- [x] table
- [x] tr
- [x] td
- [x] th
- [x] colspan
- [x] rowspan

---

## Forms

- [x] form
- [x] input
- [x] textarea
- [x] select
- [x] option
- [x] optgroup
- [x] button
- [x] validation

---

## Multimedia

- [x] audio
- [x] video
- [x] source
- [x] picture

---

## Semantic HTML

- [x] header
- [x] nav
- [x] main
- [x] section
- [x] article
- [x] aside
- [x] footer

---

## Advanced

- [x] iframe
- [x] HTML Entities
- [x] Meta Tags
- [x] Accessibility
- [x] Best Practices

---

# 🎉 Congratulations!

You have successfully completed the **HTML Course**.

You are now ready to start **CSS**.

---

## Final Progress

```text
HTML Roadmap

████████████████████████████████████

100% Completed ✅
```

## What's Next?

➡️ **CSS Day 1**

- Introduction to CSS
- Inline CSS
- Internal CSS
- External CSS
- CSS Syntax
- Selectors
- Colors
- Backgrounds







---

pleted
