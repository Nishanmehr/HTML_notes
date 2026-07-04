# 📘 Day 01 - HTML Foundations

> Goal: Understand how HTML works and build a strong foundation before moving to advanced topics.

---

# 📑 Table of Contents

- Introduction to HTML
- What is HyperText?
- What is Markup?
- Why HTML?
- HTML vs Programming Language
- How the Web Works
- HTML Document Structure
- HTML Tags vs Elements
- Empty (Void) Elements
- Attributes
- Comments

---

# 1. Introduction to HTML

## What is HTML?

**HTML (HyperText Markup Language)** is the standard markup language used to create the **structure** of a webpage.

HTML tells the browser:

- What is a heading
- What is a paragraph
- What is a list
- What is a table
- What is an image
- What is a link

HTML does **not** add styling or logic.

---

## What does HyperText mean?

HyperText means text that can connect one document to another using hyperlinks.

Example:

```
Google
   ↓
Click
   ↓
Gmail
```

This connection is created using the `<a>` tag.

---

## What does Markup mean?

Markup means describing content using tags.

Example:

```html
<h1>Nishant Mehra</h1>
```

The browser understands this is a heading.

Without tags:

```
Nishant Mehra
```

The browser only sees plain text.

---

## Why do we use HTML?

Without HTML:

```
Nishant Mehra
Software Engineer
```

Everything appears as plain text.

With HTML:

```html
<h1>Nishant Mehra</h1>
<h2>Software Engineer</h2>
<p>I love Web Development.</p>
```

The browser can understand the structure of the webpage.

---

## HTML vs Programming Language

| HTML | Programming Language |
|------|-----------------------|
| Markup Language | Programming Language |
| Creates Structure | Performs Logic |
| No Loops | Supports Loops |
| No Conditions | Supports Conditions |
| No Variables | Supports Variables |

Examples of Programming Languages:

- Java
- Python
- JavaScript
- C++
- C#

---

# 2. How the Web Works

```
User
   │
   ▼
Browser
   │
HTTP Request
   │
   ▼
Server
   │
Returns HTML
   │
   ▼
Browser Reads HTML
   │
Top → Bottom
   │
Displays Webpage
```

### Important Points

- Browser requests a webpage.
- Server sends an HTML document.
- Browser reads HTML **from top to bottom**.
- Browser only understands HTML tags.
- Browser ignores comments.

---

# 3. HTML Document Structure

Every HTML page starts with the following structure.

```html
<!DOCTYPE html>
<html lang="en">

<head>

</head>

<body>

</body>

</html>
```

---

## `<!DOCTYPE html>`

Purpose:

- Tells the browser that this is an HTML5 document.
- Prevents Quirks Mode.

> Interview Point:
> `<!DOCTYPE html>` is a declaration, **not** an HTML tag.

---

## `<html>`

Root element of the webpage.

Everything must be written inside it.

Example:

```html
<html lang="en">

</html>
```

---

## `lang="en"`

- `lang` → Attribute
- `en` → Value

Purpose:

- Specifies the language of the webpage.
- Helps SEO.
- Helps screen readers.
- Improves accessibility.

---

## `<head>`

Contains metadata.

Metadata means information **about** the webpage.

Examples:

- Title
- Meta Tags
- CSS Links
- JavaScript Files

Content inside `<head>` is generally **not visible** on the webpage.

---

## `<title>`

Appears on the browser tab.

Example:

```html
<title>My Portfolio</title>
```

---

## `<body>`

Contains everything visible on the webpage.

Examples:

- Headings
- Paragraphs
- Images
- Tables
- Lists
- Forms
- Links

---

# 4. Tags vs Elements

Example:

```html
<p>Hello World</p>
```

Opening Tag

```html
<p>
```

Content

```
Hello World
```

Closing Tag

```html
</p>
```

Together they form an **HTML Element**.

---

# 5. Empty (Void) Elements

Some elements do not contain content.

Examples:

```html
<br>
<hr>
<img>
<meta>
<link>
<input>
```

These elements do not require closing tags.

Example:

```html
<br>
```

Correct ✅

```html
<br></br>
```

Incorrect ❌

---

# 6. Attributes

Attributes provide additional information about an element.

Example:

```html
<a href="https://google.com">
```

Here:

Attribute:

```
href
```

Value:

```
https://google.com
```

Another Example:

```html
<html lang="en">
```

Attribute:

```
lang
```

Value:

```
en
```

---

## Attribute Syntax

```html
<tag attribute="value">
```

Examples:

```html
<img src="profile.png">

<a href="https://google.com">

<td colspan="2">

<input type="text">
```

---

# 7. Comments

Syntax:

```html
<!-- This is a comment -->
```

Purpose:

- Explain code
- Organize sections
- Help other developers
- Temporarily disable code

The browser ignores comments.

---

# Best Practices

✅ Use meaningful comments.

Good:

```html
<!-- Education Section -->
```

Bad:

```html
<!-- Hello -->
```

---

# Common Mistakes

❌ Forgetting `<!DOCTYPE html>`

❌ Writing content outside `<body>`

❌ Forgetting closing tags (except void elements)

❌ Wrong indentation

---

# Interview Questions

1. What is HTML?
2. Why is HTML called a Markup Language?
3. Difference between HTML and Programming Languages?
4. What is HyperText?
5. What is Markup?
6. What is `<!DOCTYPE html>`?
7. What happens if we remove `<!DOCTYPE html>`?
8. What is the purpose of `<html>`?
9. Why do we use `lang="en"`?
10. What is metadata?
11. Difference between `<head>` and `<body>`?
12. What is the purpose of the `<title>` tag?
13. Difference between a tag and an element?
14. What are attributes?
15. What is an empty (void) element?
16. Why doesn't `<br>` have a closing tag?
17. What is the syntax of an attribute?
18. What are HTML comments?
19. Does the browser execute comments?
20. Why are comments useful?

---

# Summary

- HTML is a Markup Language.
- Browser reads HTML from top to bottom.
- `<!DOCTYPE html>` declares an HTML5 document.
- `<html>` is the root element.
- `<head>` stores metadata.
- `<body>` stores visible content.
- Elements are made using tags.
- Attributes provide additional information.
- Comments improve code readability.


### Part -2
# 8. Headings

HTML provides **6 heading tags**.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

Output:

```
Heading 1 (Largest)

Heading 2

Heading 3

Heading 4

Heading 5

Heading 6 (Smallest)
```

---

## Why do we use Headings?

Headings help us:

- Organize content
- Improve readability
- Improve SEO
- Help screen readers understand page structure

Example:

```
Portfolio
│
├── About Me
├── Education
├── Skills
├── Projects
└── Contact
```

Without headings, the page becomes difficult to understand.

---

## Heading Hierarchy

Correct:

```html
<h1>Portfolio</h1>

<h2>About Me</h2>

<h2>Education</h2>

<h2>Projects</h2>

<h3>Frontend Projects</h3>

<h3>Backend Projects</h3>
```

Wrong:

```html
<h1>Portfolio</h1>

<h4>About</h4>
```

Skipping heading levels is not a good practice.

---

## Can we use multiple `<h1>` tags?

Technically:

✅ Yes

Best Practice:

Use **one `<h1>`** that represents the main topic of the page.

---

## Best Practices

✅ One `<h1>` per page

✅ Maintain heading hierarchy

✅ Don't use headings just to make text bigger

---

## Common Mistakes

❌ Using headings for styling

❌ Skipping heading levels

❌ Using many `<h1>` tags unnecessarily

---

# 9. Paragraph

Paragraphs are created using the `<p>` tag.

Syntax:

```html
<p>
    This is a paragraph.
</p>
```

Purpose:

Used for writing paragraphs of text.

Example:

```html
<p>
I am a Software Engineer.
</p>
```

---

## Why not use `<br>` repeatedly?

Wrong:

```html
Line 1
<br>
Line 2
<br>
Line 3
```

Correct:

```html
<p>First Paragraph</p>

<p>Second Paragraph</p>
```

Use `<p>` when the content is a new paragraph.

Use `<br>` only when you want a line break inside the same paragraph.

---

# Difference between `<p>` and `<br>`

| `<p>` | `<br>` |
|-------|---------|
| Creates a paragraph | Breaks a line |
| Block Element | Inline (Void) Element |
| Starts on a new line | Continues in the same paragraph |

Example:

```html
<p>
Hello
<br>
World
</p>
```

Output:

```
Hello
World
```

Still one paragraph.

---

# 10. Horizontal Rule

Syntax:

```html
<hr>
```

Purpose:

Creates a horizontal line.

Used to separate content.

Example:

```
About Me
----------------------

Education
----------------------

Projects
```

---

## Why use `<hr>`?

Makes sections visually separated.

Improves readability.

---

## Common Mistakes

❌ Using many `<br>` tags instead of `<hr>`

---

# 11. Text Formatting Tags

These tags change the meaning or appearance of text.

---

## `<b>`

Purpose:

Makes text bold.

```html
<b>HTML</b>
```

Output:

**HTML**

---

## `<strong>`

Purpose:

Marks important text.

Default browser appearance:

**Bold**

```html
<strong>Important</strong>
```

### Difference

`<b>`

Only changes appearance.

`<strong>`

Adds meaning + importance.

Better for SEO and Accessibility.

---

## `<i>`

Purpose:

Displays italic text.

```html
<i>HTML</i>
```

---

## `<em>`

Purpose:

Adds emphasis to text.

Default browser appearance:

Italic

Difference:

`<i>` → Appearance

`<em>` → Meaning + Emphasis

---

## `<u>`

Purpose:

Underlines text.

```html
<u>HTML</u>
```

---

## `<mark>`

Purpose:

Highlights text.

```html
<mark>JavaScript</mark>
```

---

## `<small>`

Purpose:

Displays smaller text.

Mostly used for:

- Copyright
- Notes
- Disclaimers

Example:

```html
<small>Copyright © 2026</small>
```

---

## `<del>`

Purpose:

Represents deleted content.

Example:

```html
Old CGPA:
<del>8.5</del>

New CGPA:
8.8
```

---

## `<sub>`

Purpose:

Subscript

Mostly used for chemical formulas.

Example:

```html
H<sub>2</sub>O
```

Output:

H₂O

---

## `<sup>`

Purpose:

Superscript

Used for powers.

Example:

```html
2<sup>3</sup>
```

Output:

2³

---

# Best Practices

✅ Use `<strong>` instead of `<b>` when the text is important.

✅ Use `<em>` instead of `<i>` when emphasizing text.

✅ Use formatting tags only when required.

---

# Common Mistakes

❌ Using `<br>` to create paragraphs

❌ Using `<b>` everywhere

❌ Using formatting tags only for decoration

---

# Interview Questions

1. Why do we use headings?
2. How many heading tags are there?
3. Can we use multiple `<h1>` tags?
4. Difference between `<p>` and `<br>`?
5. Difference between `<b>` and `<strong>`?
6. Difference between `<i>` and `<em>`?
7. Why is `<strong>` better for SEO?
8. What is the use of `<mark>`?
9. Where is `<small>` commonly used?
10. What is `<del>`?
11. Difference between `<sub>` and `<sup>`?
12. What is the purpose of `<hr>`?

---

# Summary

- HTML provides six heading tags (`<h1>`–`<h6>`).
- Headings improve SEO, accessibility, and readability.
- `<p>` creates a new paragraph, while `<br>` only breaks a line.
- `<hr>` separates sections of a webpage.
- `<strong>` and `<em>` provide semantic meaning in addition to formatting.
- `<sub>` is used for chemical formulas.
- `<sup>` is used for mathematical powers.
- `<small>` is commonly used for copyright notices and additional information.




### Part 3
# 12. HTML Lists

Lists are used to display related items in an organized manner.

There are **two main types** of lists in HTML:

1. Ordered List (`<ol>`)
2. Unordered List (`<ul>`)

Both use the `<li>` (List Item) tag.

---

# Unordered List (`<ul>`)

An unordered list displays items using **bullet points**.

### Syntax

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

Output:

```
• HTML
• CSS
• JavaScript
```

### When to use?

Use an unordered list when the order of items **does not matter**.

Examples:

- Skills
- Hobbies
- Technologies
- Tools

---

# Ordered List (`<ol>`)

An ordered list displays items in a specific order.

### Syntax

```html
<ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
```

Output:

```
1. HTML
2. CSS
3. JavaScript
```

### When to use?

Use an ordered list when the order **is important**.

Examples:

- Instructions
- Recipe Steps
- Ranking
- Algorithm Steps

---

# `<li>` (List Item)

The `<li>` tag represents a single item in a list.

Example:

```html
<ul>
    <li>Java</li>
    <li>Python</li>
</ul>
```

---

## Can `<li>` exist alone?

❌ No.

`<li>` must always be inside:

- `<ul>`
- `<ol>`

---

## Difference between `<ul>` and `<ol>`

| `<ul>` | `<ol>` |
|---------|---------|
| Unordered List | Ordered List |
| Uses bullets | Uses numbers |
| Order doesn't matter | Order matters |

---

## Best Practices

✅ Use `<ul>` for skills and technologies.

✅ Use `<ol>` for step-by-step instructions.

---

# 13. HTML Links

Links are created using the `<a>` tag.

`a` stands for **Anchor**.

---

## Why do we use Links?

Links connect one page to another.

Examples:

- Portfolio
- GitHub
- LinkedIn
- Contact Page

Without links, websites would not be connected.

---

## Syntax

```html
<a href="https://github.com">GitHub</a>
```

Output:

```
GitHub
```

(clickable)

---

# `href`

`href` stands for:

**Hypertext Reference**

It specifies the destination of the link.

Example:

```html
<a href="https://google.com">
    Google
</a>
```

---

## Absolute URL

Uses the complete web address.

Example:

```html
<a href="https://github.com">
```

---

## Relative URL

Used to open pages inside the same project.

Example:

```html
<a href="about.html">
```

No complete website address is required.

---

## Best Practices

✅ Use meaningful link text.

Good:

```html
<a href="resume.pdf">
    Download Resume
</a>
```

Bad:

```html
<a href="resume.pdf">
    Click Here
</a>
```

---

# 14. HTML Images

Images are displayed using the `<img>` tag.

`<img>` is a **Void (Empty) Element**, so it does **not** require a closing tag.

---

## Syntax

```html
<img src="profile.jpg" alt="Profile Picture">
```

---

# `src`

`src` stands for:

**Source**

It specifies the location of the image.

Example:

```html
<img src="images/profile.jpg">
```

---

# `alt`

`alt` stands for:

**Alternative Text**

If the image fails to load, the browser displays the alternative text instead.

Example:

```html
<img
    src="profile.jpg"
    alt="Nishant Mehra Profile Picture">
```

---

## Why is `alt` important?

- Improves accessibility.
- Helps screen readers.
- Displays text if the image is missing.
- Improves SEO.

---

# Relative Path vs Absolute Path

## Relative Path

Refers to files inside your own project.

Example:

```html
<img src="images/profile.jpg">
```

Folder Structure:

```
Project/
│
├── index.html
│
└── images/
      └── profile.jpg
```

---

## Absolute Path

Uses the complete URL of an image hosted elsewhere.

Example:

```html
<img src="https://example.com/profile.jpg">
```

---

## Difference

| Relative Path | Absolute Path |
|---------------|---------------|
| Inside your project | External website |
| Faster | Depends on external server |
| Works offline | Requires internet |

---

# Common Mistakes

❌ Forgetting the `alt` attribute.

❌ Using spaces in image names.

Bad:

```
My Image.png
```

Good:

```
my-image.png
```

---

# Interview Questions

### Lists

1. What is the difference between `<ul>` and `<ol>`?
2. What is `<li>`?
3. Can `<li>` exist without `<ul>` or `<ol>`?

### Links

4. What is the purpose of the `<a>` tag?
5. What does `href` stand for?
6. Difference between Relative and Absolute URLs?

### Images

7. Why is `<img>` a void element?
8. What is the purpose of `src`?
9. What is the purpose of `alt`?
10. Why is `alt` important?

---

# Summary

- `<ul>` creates unordered lists.
- `<ol>` creates ordered lists.
- `<li>` represents list items.
- `<a>` creates hyperlinks.
- `href` specifies the destination of a link.
- `<img>` displays images.
- `src` specifies the image location.
- `alt` provides alternative text if the image cannot be displayed.
- Relative paths are used for project files.
- Absolute paths use complete URLs.


### Part 4

# 15. Block vs Inline Elements

Every HTML element has a default display behavior.

There are two main types:

1. Block Elements
2. Inline Elements

---

# Block Elements

A block element always starts on a **new line** and occupies the **full available width**.

Example:

```html
<h1>Hello</h1>
<p>Paragraph</p>
```

Output:

```
Hello

Paragraph
```

Even if there is space, the next block element starts on a new line.

---

## Common Block Elements

```html
<h1> - <h6>
<p>
<div>
<ul>
<ol>
<li>
<table>
<form>
<header>
<footer>
<section>
<nav>
<main>
```

---

# Inline Elements

Inline elements occupy **only the space they need**.

They do **not** start on a new line.

Example:

```html
I know <strong>HTML</strong> and <mark>CSS</mark>.
```

Output:

```
I know HTML and CSS.
```

---

## Common Inline Elements

```html
<a>
<span>
<strong>
<b>
<em>
<i>
<mark>
<small>
<sub>
<sup>
<br>
<img>
```

---

# Difference Between Block and Inline

| Block Element | Inline Element |
|---------------|----------------|
| Starts on a new line | Does not start on a new line |
| Takes full width | Takes only required width |
| Can contain block and inline elements (depending on HTML rules) | Usually contains text or inline content |

---

# 16. `<div>` vs `<span>`

Both are generic container elements.

Neither adds styling by itself.

---

# `<div>`

The `<div>` element is a **block-level container**.

It is used to group large sections of a webpage.

Example:

```html
<div>
    <h2>About Me</h2>
    <p>I am a Software Engineer.</p>
</div>
```

Use `<div>` to wrap:

- Sections
- Cards
- Forms
- Navigation
- Layout containers

---

# `<span>`

The `<span>` element is an **inline container**.

It is used to wrap a small part of text.

Example:

```html
<p>
I know <span>Java</span>.
</p>
```

Use `<span>` when you want to target or highlight a word or small phrase.

---

# Difference Between `<div>` and `<span>`

| `<div>` | `<span>` |
|----------|-----------|
| Block Element | Inline Element |
| Wraps large sections | Wraps small text |
| Starts on a new line | Stays in the same line |

---

# Semantic vs Non-Semantic Elements

Semantic elements describe the **meaning** of the content.

Examples:

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

Non-semantic elements do **not** describe their purpose.

Examples:

```html
<div>
<span>
```

We will study semantic elements in detail on **Day 2**.

---

# Best Practices

- Use only one `<h1>` per page.
- Follow heading hierarchy (`<h1>` → `<h2>` → `<h3>`).
- Use `<strong>` and `<em>` when meaning is important.
- Always add the `alt` attribute to images.
- Use meaningful comments.
- Keep code properly indented.
- Use relative paths for project files whenever possible.
- Use `<div>` for grouping sections and `<span>` for small pieces of text.

---

# Common Mistakes

- Forgetting `<!DOCTYPE html>`.
- Writing content outside the `<body>`.
- Using `<li>` without `<ul>` or `<ol>`.
- Using `<br>` to create large spaces.
- Forgetting the `alt` attribute on images.
- Typing `<spam>` instead of `<span>`.
- Placing block elements inside `<p>`.
- Using headings only to make text look bigger.

---

# Revision Cheat Sheet

## Document Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>My Website</title>
</head>
<body>

</body>
</html>
```

---

## Headings

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
```

---

## Paragraph

```html
<p>This is a paragraph.</p>
```

---

## Line Break

```html
<br>
```

---

## Horizontal Line

```html
<hr>
```

---

## Lists

```html
<ul>
    <li>HTML</li>
</ul>

<ol>
    <li>Step 1</li>
</ol>
```

---

## Link

```html
<a href="https://example.com">
    Visit Website
</a>
```

---

## Image

```html
<img src="profile.jpg" alt="Profile Picture">
```

---

## Formatting

```html
<strong>Important</strong>

<em>Emphasis</em>

<mark>Highlight</mark>

<small>Small Text</small>

<sub>2</sub>

<sup>3</sup>

<del>Deleted</del>
```

---

## Containers

```html
<div>

</div>

<span>

</span>
```

---

# Interview Questions

### Theory

1. What is HTML?
2. Why is HTML called a Markup Language?
3. Explain the structure of an HTML document.
4. Difference between tags and elements.
5. What are attributes?
6. What is `<!DOCTYPE html>`?
7. Difference between `<head>` and `<body>`.
8. What is metadata?
9. Difference between `<b>` and `<strong>`.
10. Difference between `<i>` and `<em>`.
11. Difference between `<p>` and `<br>`.
12. Difference between `<ul>` and `<ol>`.
13. Can `<li>` exist alone?
14. What is the purpose of `href`?
15. Difference between relative and absolute paths.
16. What is the purpose of the `alt` attribute?
17. Why is `<img>` a void element?
18. Difference between block and inline elements.
19. Difference between `<div>` and `<span>`.
20. What are semantic and non-semantic elements?

### Output-Based Questions

1. Predict the output of nested headings.
2. Predict the output of `<br>` inside a paragraph.
3. Predict the output of nested lists.
4. Identify errors in a broken HTML document.
5. Find mistakes in an image tag.
6. Find mistakes in a link tag.
7. Predict the output of `<mark>`, `<del>`, and `<small>`.
8. Identify whether an element is block or inline.
9. Explain what happens if `alt` is omitted.
10. Find the mistake in `<spam>` vs `<span>`.
11. Correct an invalid list structure.
12. Correct an invalid paragraph containing block elements.
13. Predict the output of mixed formatting tags.
14. Explain why `<!DOCTYPE html>` is important.
15. Build a small profile page using all Day 1 concepts.

---

# Day 1 Project Status

By the end of Day 1, your portfolio should include:

- Personal Introduction
- About Me
- Education
- Skills
- Projects
- Contact Information
- Social Links
- Tables (introduced early in your course)
- Proper headings and paragraphs
- Lists
- Links
- Images (to be added later)
- Good HTML structure

---

# Day 1 Completed 🎉

You now understand the fundamentals of HTML and are ready to move on to more advanced topics like **Forms**, **Semantic HTML**, **Multimedia**, and **Accessibility**.








