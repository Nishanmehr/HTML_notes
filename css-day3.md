# CSS Day 3 Notes (Flexbox Complete)

# Topics Covered

- Introduction to Flexbox
- display:flex
- justify-content
- align-items
- flex-direction
- gap
- flex-wrap
- flex-grow
- flex-shrink
- order
- align-self

---

# What is Flexbox?

Flexbox is a one-dimensional layout system.

It is used to arrange elements in

- Row
- Column

Flexbox makes layouts easy and responsive.

---

# Flex Container

Parent Element

Example

<nav class="navbar">

    <a>Home</a>

    <a>Shop</a>

</nav>

Here

navbar

↓

Flex Container

---

# Flex Items

Direct children of Flex Container.

Example

<a>

<a>

↓

Flex Items

---

# display:flex ⭐⭐⭐⭐⭐

Converts Parent into Flex Container.

Syntax

.parent{

display:flex;

}

Result

Children automatically become Flex Items.

---

# justify-content ⭐⭐⭐⭐⭐

Controls Horizontal Alignment
(Main Axis)

Syntax

justify-content:value;

Values

flex-start

center

flex-end

space-between ⭐⭐⭐⭐⭐

space-around

space-evenly

---

# space-between

First item touches left.

Last item touches right.

Equal space in between.

Best for

✔ Navbar

---

# space-around

Equal space around every item.

Edge spacing becomes half.

---

# space-evenly

Equal spacing everywhere.

---

# align-items ⭐⭐⭐⭐⭐

Controls Vertical Alignment
(Cross Axis)

Syntax

align-items:value;

Values

stretch

flex-start

center ⭐⭐⭐⭐⭐

flex-end

---

# align-items:center

Most commonly used.

Perfect for

Navbar

Cards

Buttons

Login Forms

---

# Main Axis vs Cross Axis

Default Direction

Row

Main Axis

Left → Right

Cross Axis

Top → Bottom

---

# flex-direction ⭐⭐⭐⭐⭐

Changes Flex Direction.

Syntax

flex-direction:value;

Values

row ⭐⭐⭐⭐⭐

column ⭐⭐⭐⭐⭐

row-reverse

column-reverse

---

# Row

Items appear

Left → Right

---

# Column

Items appear

Top → Bottom

---

# Important

When direction changes,

Main Axis also changes.

Row

Main Axis

Horizontal

Column

Main Axis

Vertical

---

# gap ⭐⭐⭐⭐⭐

Creates spacing between Flex Items.

Syntax

gap:value;

Example

.container{

display:flex;

gap:20px;

}

---

# row-gap

Vertical spacing only.

---

# column-gap

Horizontal spacing only.

---

# gap:20px 40px;

20px

↓

Row Gap

40px

↓

Column Gap

---

# Gap vs Margin

Gap

✔ Parent Property

✔ Cleaner

✔ Professional

Margin

Applied on Child

Less preferred for Flex layouts

---

# flex-wrap ⭐⭐⭐⭐⭐

Controls whether items move to next line.

Syntax

flex-wrap:value;

Values

nowrap ⭐⭐⭐⭐⭐ (Default)

wrap ⭐⭐⭐⭐⭐

wrap-reverse

---

# nowrap

Everything remains in one line.

---

# wrap

Moves items to next line automatically.

Used in

Product Cards

Gallery

Dashboard

---

# Professional Combination

display:flex;

flex-wrap:wrap;

gap:20px;

---

# flex-grow ⭐⭐⭐⭐⭐

Decides which item gets extra available space.

Child Property

Syntax

.item{

flex-grow:value;

}

---

# flex-grow:1

Item takes available extra space.

---

# flex-grow:2

Gets double extra space compared to

flex-grow:1

---

# Used In

Navbar

Sidebar

Dashboard

Cards

---

# flex-shrink ⭐⭐⭐⭐⭐

Decides how item shrinks when space becomes less.

Child Property

Syntax

.item{

flex-shrink:value;

}

---

# Default

flex-shrink:1;

---

# flex-shrink:0

Item never shrinks.

Best for

Logo

Images

Icons

---

# order ⭐⭐⭐⭐⭐

Changes display order without changing HTML.

Child Property

Syntax

.item{

order:value;

}

---

# Default

order:0;

---

# order:-1

Moves item before all default items.

---

# Smaller order

Appears First

Larger order

Appears Later

---

# align-self ⭐⭐⭐⭐⭐

Changes alignment of one specific Flex Item.

Child Property

Syntax

.item{

align-self:value;

}

Values

auto

flex-start

center

flex-end

stretch

---

# Difference

align-items

Parent Property

Affects all children.

align-self

Child Property

Affects only one child.

---

# Parent Properties ⭐⭐⭐⭐⭐

display:flex;

justify-content;

align-items;

flex-direction;

gap;

flex-wrap;

---

# Child Properties ⭐⭐⭐⭐⭐

flex-grow;

flex-shrink;

order;

align-self;

---

# 80/20 Flexbox Properties

These are used in almost every project.

display:flex;

justify-content:space-between;

align-items:center;

gap:20px;

flex-wrap:wrap;

---

# Most Used Navbar

.navbar{

display:flex;

justify-content:space-between;

align-items:center;

}

---

# Product Cards

.products{

display:flex;

flex-wrap:wrap;

gap:20px;

}

---

# Interview Questions

Q. What is Flexbox?

One-dimensional layout system.

---

Q. Difference between Flex Container and Flex Item?

Container

Parent

Item

Direct Child

---

Q. display:flex kis par lagta hai?

Parent

---

Q. justify-content kis axis par kaam karta hai?

Main Axis

---

Q. align-items kis axis par kaam karta hai?

Cross Axis

---

Q. Default flex-direction?

row

---

Q. Default flex-wrap?

nowrap

---

Q. Default order?

0

---

Q. Default flex-shrink?

1

---

Q. Difference between flex-grow and flex-shrink?

flex-grow

Distributes Extra Space

flex-shrink

Shrinks when space is less

---

Q. Difference between align-items and align-self?

align-items

Parent Property

All children

align-self

Child Property

Single child

---

# Best Practices

✔ Use Flexbox for layouts.

✔ Use gap instead of margin.

✔ Use wrap for product cards.

✔ Use align-items:center for navbar.

✔ Use flex-grow for dashboards.

✔ Use flex-shrink:0 for logo and images.

✔ Keep HTML semantic.

---

# Common Mistakes

❌ Applying display:flex on child.

❌ Using gap on child.

❌ Confusing Main Axis and Cross Axis.

❌ Using order unnecessarily.

❌ Using flex-grow on parent.

❌ Using align-self on parent.

---

# Real World Usage

Navbar

display:flex;

justify-content:space-between;

align-items:center;

Hero Section

display:flex;

align-items:center;

Product Section

display:flex;

flex-wrap:wrap;

gap:20px;

Dashboard

display:flex;

Sidebar

flex-grow:1;

Content

flex-grow:4;

---

# ShopEase Progress

✅ HTML Completed

✅ Basic CSS Styling Completed

✅ Colors

✅ Typography Basics

✅ Selectors

✅ Box Model

✅ Padding

✅ Margin

✅ Display

✅ Position

✅ Overflow

✅ Flexbox Complete

---

# CSS Course Progress (5-Day Plan)

Day 1 ✅

Introduction

Selectors

Colors

Units

Background

Borders

Width & Height

---

Day 2 ✅

Box Model

Padding

Margin

Display

Position

Overflow

---

Day 3 ✅

Flexbox Complete

---

Day 4 ⬜

CSS Grid

Typography

Shadows

Gradients

Transitions

Transform

---

Day 5 ⬜

Animations

Responsive Design

Media Queries

Variables

Pseudo Classes

Pseudo Elements

Advanced Selectors

Final ShopEase Redesign

---

Overall Progress

✅ 60% Completed
