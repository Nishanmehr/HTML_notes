# CSS Day 1 Notes

# Topics Covered

- Introduction to CSS
- Ways to Add CSS
- Element Selector
- Class Selector
- Colors
- Units
- Backgrounds
- Borders
- Width & Height

---

# 1. What is CSS?

CSS (Cascading Style Sheets) is used to style HTML elements.

HTML = Structure
CSS = Design

Example:

HTML

<h1>ShopEase</h1>

CSS

h1{
    color: blue;
}

Output:
The heading becomes blue.

---

# 2. Ways to Add CSS

## 1. Inline CSS

<h1 style="color:red;">ShopEase</h1>

✔ Used for testing
❌ Not recommended

---

## 2. Internal CSS

<head>
<style>

h1{
    color:red;
}

</style>
</head>

✔ Small projects

---

## 3. External CSS ⭐⭐⭐⭐⭐

HTML

<link rel="stylesheet" href="../css/style.css">

CSS

h1{
    color:red;
}

✔ Professional method
✔ Reusable
✔ Easy to maintain

---

# CSS File Linking

If HTML and CSS are in different folders

Project

HomePage/
│
├── html/
│   └── index.html
│
├── css/
│   └── style.css

From html folder to css folder

<link rel="stylesheet" href="../css/style.css">

Meaning

..

Go one folder back.

css/

Go inside css folder.

style.css

Open style.css

---

# 3. Element Selector

Syntax

selector{

    property:value;

}

Example

h1{

    color:red;

}

Output

All h1 become red.

Example

button{

    background-color:black;

}

All buttons become black.

---

# 4. Class Selector ⭐⭐⭐⭐⭐

Used when we want to style specific elements.

HTML

<h1 class="hero-heading">
Elevate Your Style
</h1>

CSS

.hero-heading{

    font-size:48px;

}

Rules

Class starts with

.

Example

.hero

.logo

.navbar

.hero-image

Professional Naming

✔ hero-heading
✔ product-card
✔ nav-link
✔ hero-image

Avoid

❌ abc
❌ xyz
❌ test123

---

# 5. Colors

## Text Color

color

Example

h1{

    color:#000000;

}

---

## Background Color

background-color

Example

button{

    background-color:#000000;

}

---

## Common Color Formats

HEX ⭐⭐⭐⭐⭐

#ffffff

White

#000000

Black

#ff0000

Red

#00ff00

Green

RGB

rgb(255,0,0)

RGBA

rgba(0,0,0,0.5)

---

# Difference

color

Changes text color.

background-color

Changes background color.

---

# 6. Units

## px

Fixed unit

Example

width:300px;

font-size:20px;

---

## %

Relative to parent

Example

width:50%;

---

## rem

Relative to root font size.

1rem = 16px

2rem = 32px

---

## em

Relative to parent font size.

(Will study in Typography.)

---

## vw

Viewport Width

100vw

Full screen width

---

## vh

Viewport Height

100vh

Full screen height

---

# 7. Backgrounds

## Background Color

.hero{

    background-color:#fdf8f3;

}

---

## Background Image

.hero{

    background-image:url("../images/bg.jpg");

}

---

## Prevent Repeating

background-repeat:no-repeat;

---

## Cover Entire Area

background-size:cover;

---

## Center Image

background-position:center;

---

# 8. Borders

Syntax

border:2px solid black;

Breakdown

2px

Border thickness

solid

Border style

black

Border color

---

Border Styles

solid

dashed

dotted

double

---

Rounded Corners

border-radius:8px;

Circle

border-radius:50%;

---

# 9. Width & Height

Width

width:300px;

Height

height:200px;

Example

.hero-image{

    width:450px;

}

button{

    width:180px;

    height:45px;

}

---

# Important Rules

✔ HTML = Structure

✔ CSS = Design

Don't write

<img width="300">

Instead

<img class="hero-image">

CSS

.hero-image{

    width:300px;

}

---

# Project Classes Used

.header

.navbar

.logo

.nav-link

.nav-icon

.hero

.hero-heading

.hero-image

.btn

.product-card

.product-image

.footer

---

# Best Practices

✔ Use External CSS

✔ Use meaningful class names

✔ Prefer HEX colors

✔ Keep design in CSS

✔ Don't style everything with element selectors

✔ Use class selectors for project components

---

# Day 1 Progress

✅ Introduction

✅ Ways to Add CSS

✅ Element Selector

✅ Class Selector

✅ Colors

✅ Units

✅ Backgrounds

✅ Borders

✅ Width & Height

Day 1 Completed = 100%

---

# What's Next?

Day 2

- Box Model
- Margin
- Padding
- Display
- Position
- Overflow

After Day 2, the ShopEase layout will start matching the reference design.
