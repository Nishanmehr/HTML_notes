# CSS Day 2 Notes

# Topics Covered

- Box Model
- Padding
- Margin
- Display
- Position
- Overflow

---

# 1. CSS Box Model ⭐⭐⭐⭐⭐

Every HTML element is treated as a Box.

Each box has 4 parts.

+----------------------------+
|          Margin            |
|  +----------------------+  |
|  |       Border         |  |
|  |  +----------------+  |  |
|  |  |    Padding     |  |  |
|  |  | +------------+ |  |  |
|  |  | |  Content   | |  |  |
|  |  | +------------+ |  |  |
|  |  +----------------+  |  |
|  +----------------------+  |
+----------------------------+

---

## Content

The actual text or image.

Example

<button>Shop Now</button>

Content = Shop Now

---

## Padding

Space inside the border.

Example

button{
    padding:20px;
}

Result

The text moves away from the border.

---

## Border

The line around the element.

Example

button{
    border:2px solid black;
}

---

## Margin

Space outside the element.

Example

button{
    margin:20px;
}

Creates distance from nearby elements.

---

# Padding vs Margin

Padding

✔ Inside Space

Margin

✔ Outside Space

Easy Trick

Padding = Inside

Margin = Outside

---

# 2. Padding ⭐⭐⭐⭐⭐

Padding creates space inside an element.

Syntax

selector{

    padding:value;

}

Example

button{

    padding:20px;

}

---

## Different Ways

### Same on all sides

padding:20px;

Top = Right = Bottom = Left = 20px

---

### Top-Bottom | Left-Right

padding:20px 40px;

Top = Bottom = 20px

Left = Right = 40px

---

### Clockwise Rule ⭐⭐⭐⭐⭐

padding:10px 20px 30px 40px;

Top = 10px

Right = 20px

Bottom = 30px

Left = 40px

Remember

Top → Right → Bottom → Left

---

### Individual Sides

padding-top:20px;

padding-right:30px;

padding-bottom:20px;

padding-left:30px;

---

# 3. Margin ⭐⭐⭐⭐⭐

Margin creates space outside the element.

Syntax

selector{

    margin:value;

}

---

## Same on all sides

margin:20px;

---

## Top-Bottom | Left-Right

margin:20px 40px;

---

## Clockwise Rule

margin:10px 20px 30px 40px;

Top

Right

Bottom

Left

---

## Individual Sides

margin-top:20px;

margin-right:20px;

margin-bottom:20px;

margin-left:20px;

---

# Difference

Padding

Inside Space

Margin

Outside Space

---

# 4. Display ⭐⭐⭐⭐⭐

Controls how an element behaves.

Syntax

display:value;

---

## Block

Examples

h1

p

section

div

Characteristics

✔ Starts from a new line

✔ Takes full width

Example

display:block;

---

## Inline

Examples

a

span

strong

Characteristics

✔ Does not start from a new line

✔ Takes only required width

Example

display:inline;

---

## Inline-Block ⭐⭐⭐⭐⭐

Combination of Block and Inline.

✔ Stays in same line

✔ Width works

✔ Height works

Example

display:inline-block;

---

## None

display:none;

Element disappears.

Still exists in HTML.

---

# 5. Position ⭐⭐⭐⭐⭐

Controls element location.

Syntax

position:value;

---

## Static

Default value.

position:static;

---

## Relative

Moves from original position.

Example

position:relative;

left:20px;

top:20px;

---

## Absolute

Removes element from normal flow.

Placed relative to nearest positioned parent.

Example

position:absolute;

top:20px;

right:20px;

---

## Fixed

Stays fixed while scrolling.

Example

position:fixed;

top:0;

---

## Position Properties

top

right

bottom

left

These work with

relative

absolute

fixed

sticky

---

# 6. Overflow ⭐⭐⭐⭐⭐

Controls what happens when content is larger than the container.

Syntax

overflow:value;

---

## Visible (Default)

overflow:visible;

Extra content remains visible.

---

## Hidden

overflow:hidden;

Extra content gets hidden.

---

## Scroll

overflow:scroll;

Always shows scrollbar.

---

## Auto ⭐⭐⭐⭐⭐

overflow:auto;

Scrollbar appears only if needed.

Most commonly used.

---

## Horizontal Overflow

overflow-x:auto;

---

## Vertical Overflow

overflow-y:auto;

---

# Commonly Used Properties

padding

padding-top

padding-right

padding-bottom

padding-left

margin

margin-top

margin-right

margin-bottom

margin-left

display

position

overflow

width

height

border

border-radius

---

# Interview Questions

## Difference between Padding and Margin?

Padding

Inside spacing

Margin

Outside spacing

---

## Difference between Block and Inline?

Block

Starts from new line

Takes full width

Inline

Does not start from new line

Takes only required width

---

## Which display value allows width and height while staying in one line?

inline-block

---

## Difference between Relative and Absolute?

Relative

Moves from original position.

Absolute

Removed from normal document flow.

---

## Which overflow value is mostly used?

overflow:auto;

---

# Best Practices

✔ Use Padding for internal spacing.

✔ Use Margin for external spacing.

✔ Use inline-block when width and height are needed.

✔ Use auto instead of scroll.

✔ Use Position only when necessary.

✔ Prefer Flexbox for layouts.

---

# Common Mistakes

❌ Using Margin instead of Padding.

❌ Using Absolute for entire page layout.

❌ Using Scroll everywhere.

❌ Forgetting the Clockwise Rule.

❌ Confusing Block and Inline elements.

---

# Professional Tips

✔ Layout → Flexbox/Grid

✔ Floating Badge → Position

✔ Sticky Navbar → Fixed/Sticky

✔ Internal Spacing → Padding

✔ External Spacing → Margin

✔ Responsive Layout → Flexbox

---

# Project Progress

Day 1

✔ Completed

Day 2

✔ Completed

Current Project

✔ Basic Styling Done

✔ Hero Section Improved

✔ Buttons Styled

✔ Understanding of CSS Layout Started

---

# CSS Course Progress (5-Day Plan)

Day 1 ✅

Day 2 ✅

Day 3 ⬜ Flexbox (Complete)

Day 4 ⬜ Grid + Typography + Shadows + Gradients + Transitions + Transform

Day 5 ⬜ Animations + Responsive Design + Media Queries + Variables + Pseudo Classes + Pseudo Elements + Advanced Selectors + Final ShopEase Project

Overall Progress

40% Completed
