# 📅 Day 2 - HTML Tables & Forms (Part 1)

---

# 📚 Topics Covered

- HTML Tables
- Table Structure
- `<thead>`, `<tbody>`, `<tfoot>`
- `colspan`
- `rowspan`
- HTML Forms
- `<form>`
- `action`
- `method`
- `<label>`
- `for`
- `<input>`
- `type`
- `id`
- `name`
- `placeholder`
- `value`

---

# HTML Tables

HTML tables are used to display data in rows and columns.

Example:

```html
<table>
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>Nishant</td>
        <td>22</td>
    </tr>
</table>
```

---

# Table Tags

| Tag | Purpose |
|------|----------|
| `<table>` | Creates a table |
| `<tr>` | Creates a table row |
| `<th>` | Table heading |
| `<td>` | Table data |

---

# Table Structure

HTML provides semantic sections for tables.

```html
<table>

    <thead>

    </thead>

    <tbody>

    </tbody>

    <tfoot>

    </tfoot>

</table>
```

---

## `<thead>`

Contains column headings.

```html
<thead>
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>
</thead>
```

---

## `<tbody>`

Contains the main table data.

```html
<tbody>
    <tr>
        <td>Nishant</td>
        <td>22</td>
    </tr>
</tbody>
```

---

## `<tfoot>`

Contains summary or footer information.

```html
<tfoot>
    <tr>
        <td colspan="2">
            Total Students : 1
        </td>
    </tr>
</tfoot>
```

---

# colspan

Used to merge multiple columns.

Syntax

```html
<td colspan="2">
```

Example

```html
<tr>
    <td colspan="2">
        Total Marks
    </td>
</tr>
```

---

# rowspan

Used to merge multiple rows.

Syntax

```html
<td rowspan="2">
```

Example

```html
<tr>
    <td rowspan="2">
        Nishant
    </td>

    <td>HTML</td>
</tr>

<tr>
    <td>CSS</td>
</tr>
```

---

# HTML Forms

HTML forms are used to collect user input and send it to a server.

Examples:

- Login Form
- Registration Form
- Contact Form
- Job Application Form

---

# `<form>`

The `<form>` tag is a container for all form elements.

```html
<form>

</form>
```

---

# action

Specifies where the form data will be sent.

```html
<form action="/login">
```

---

# method

Specifies how the data is sent.

Common methods:

- GET
- POST

Example

```html
<form action="/login" method="POST">
```

---

# `<label>`

Provides a description for an input field.

Example

```html
<label for="fullname">
    Full Name
</label>
```

---

# for Attribute

Connects a label with an input.

The value of `for` must match the input's `id`.

```html
<label for="fullname">

<input id="fullname">
```

Benefits

- Better accessibility
- Better user experience
- Clicking the label focuses the input

---

# `<input>`

Used to collect data from the user.

Example

```html
<input type="text">
```

`<input>` is a **void element**, so it has no closing tag.

---

# type Attribute

Defines what kind of input the browser should create.

Example

```html
<input type="text">
```

Default type:

```html
<input>
```

is equal to

```html
<input type="text">
```

---

# id Attribute

Uniquely identifies an HTML element.

Example

```html
<input id="fullname">
```

Best Practices

- Must be unique
- Avoid spaces
- Use lowercase

Good

```html
id="fullname"
```

Bad

```html
id="Full Name"
```

---

# name Attribute

Defines the key sent to the server.

Example

```html
<input
    name="fullname">
```

If the user enters

```
Nishant Mehra
```

The browser sends

```
fullname = Nishant Mehra
```

---

# Difference Between id and name

| id | name |
|----|------|
| Identifies HTML element | Identifies submitted data |
| Used by CSS, JavaScript and Label | Used by Server |
| Must be unique | Can repeat in some cases |

---

# placeholder

Displays a temporary hint inside an input.

Example

```html
<input
    placeholder="Enter your full name">
```

The placeholder disappears when the user starts typing.

---

# value

Provides a default value.

Example

```html
<input
    value="India">
```

Output

```
India
```

The value is submitted to the server if unchanged.

---

# placeholder vs value

| placeholder | value |
|-------------|-------|
| Temporary hint | Actual data |
| Disappears while typing | Remains until changed |
| Not submitted | Submitted |

---

# Best Practices

- Always use `<label>` with `<input>`.
- `for` should match `id`.
- Use meaningful `name` values.
- Do not use spaces in `id`.
- Use placeholder only as a hint.
- Do not replace labels with placeholders.
- Use `value` only when default data is needed.
- Use semantic table sections.

---

# Common Mistakes

❌ Using spaces in `id`

```html
id="Full Name"
```

✔ Correct

```html
id="fullname"
```

---

❌ Forgetting `name`

```html
<input id="email">
```

✔ Correct

```html
<input
    id="email"
    name="email">
```

---

❌ Using placeholder instead of label

Wrong

```html
<input
    placeholder="Email">
```

Correct

```html
<label for="email">
    Email
</label>

<input
    id="email"
    placeholder="Enter your email">
```

---

# Interview Questions

1. What is an HTML table?
2. Difference between `<th>` and `<td>`?
3. Purpose of `<thead>`, `<tbody>`, `<tfoot>`?
4. What is `colspan`?
5. What is `rowspan`?
6. What is an HTML form?
7. Purpose of the `<form>` tag?
8. Difference between `GET` and `POST`? *(Detailed later)*
9. Why do we use `<label>`?
10. Purpose of the `for` attribute?
11. What is the default type of `<input>`?
12. Why is `<input>` a void element?
13. Difference between `id` and `name`?
14. What is the purpose of `placeholder`?
15. Difference between `placeholder` and `value`?


# Progress

Day 2 Progress

```
███████████░░░░░░░░░░░░ 50%
```

## 📘 HTML Forms (Part 2)

---

# Topics Covered

- `required`
- `readonly`
- `disabled`
- `autocomplete`
- `autofocus`
- Input Types
  - `email`
  - `password`
  - `number`
  - `tel`
  - `url`

---

# required Attribute

The `required` attribute makes an input field mandatory.

The browser will not allow the form to be submitted if the field is empty.

## Syntax

```html
<input
    type="text"
    required>
```

---

## Example

```html
<label for="fullname">Full Name</label>

<input
    type="text"
    id="fullname"
    name="fullname"
    required>
```

If the user clicks **Submit** without entering a value, the browser automatically shows a validation message.

---

## Key Points

- Boolean attribute
- No value is required
- Browser performs validation
- Prevents empty submission

---

## Best Practice

✅

```html
<input required>
```

Avoid writing

```html
<input required="true">
```

---

## Interview Question

**Q. What is the purpose of the `required` attribute?**

**Answer**

It makes a form field mandatory and prevents form submission until the field contains a value.

---

# readonly Attribute

The `readonly` attribute allows the user to see the value but prevents editing.

---

## Syntax

```html
<input
    type="text"
    readonly>
```

---

## Example

```html
<input
    type="text"
    value="EMP1025"
    readonly>
```

Output

```
EMP1025
```

The user

- Can click
- Can select text
- Can copy
- Cannot edit

---

## Important Point

The value **is submitted** to the server.

---

## Real World Example

Employee ID

```
EMP1025
```

The employee should not change it, but the server still needs to receive it.

---

# disabled Attribute

The `disabled` attribute completely disables an input.

---

## Syntax

```html
<input disabled>
```

---

## Example

```html
<input
    type="text"
    value="Coming Soon"
    disabled>
```

The user

- Cannot click
- Cannot edit
- Cannot focus

---

## Important Point

Disabled inputs are **NOT submitted** to the server.

---

## Difference Between readonly and disabled

| readonly | disabled |
|-----------|----------|
| Can focus | Cannot focus |
| Can copy text | Cannot copy normally |
| Cannot edit | Cannot edit |
| Submitted to server | Not submitted |

---

## Interview Question

**Q. Difference between readonly and disabled?**

| readonly | disabled |
|-----------|----------|
| Value submitted | Value ignored |
| Clickable | Not clickable |

---

# autocomplete Attribute

Allows the browser to suggest previously entered values.

---

## Syntax

```html
<input
    autocomplete="on">
```

or

```html
<input
    autocomplete="off">
```

---

## Better Practice

Instead of

```html
autocomplete="on"
```

Use

```html
autocomplete="name"
```

Examples

```html
autocomplete="email"

autocomplete="tel"

autocomplete="street-address"

autocomplete="postal-code"
```

These help browsers autofill the correct information.

---

## Example

```html
<input
    type="email"
    autocomplete="email">
```

The browser may suggest previously saved email addresses.

---

# autofocus Attribute

Automatically places the cursor inside an input when the page loads.

---

## Syntax

```html
<input autofocus>
```

---

## Example

```html
<input
    type="text"
    autofocus>
```

When the page opens, the cursor is already inside the input field.

---

## Best Practice

Only one element on a page should normally have `autofocus`.

---

# Input Type : email

Used for email addresses.

---

## Syntax

```html
<input
    type="email">
```

---

## Example

```html
<input
    type="email"
    id="email"
    name="email">
```

The browser checks that the entered value looks like a valid email address.

Example

```
boss@gmail.com
```

Invalid

```
bossgmail.com
```

---

# Input Type : password

Used for passwords.

Characters are hidden while typing.

---

## Syntax

```html
<input
    type="password">
```

---

## Example

```html
<input
    type="password"
    id="password"
    name="password">
```

Displayed as

```
••••••••••
```

---

## Important Note

`type="password"` only hides the characters on screen.

It **does not encrypt** the password.

Security depends on HTTPS and proper server-side handling.

---

# Input Type : number

Used to accept numeric values.

---

## Syntax

```html
<input
    type="number">
```

---

## Example

```html
<input
    type="number"
    id="age"
    name="age">
```

Useful attributes

```html
min="18"

max="60"

step="1"
```

---

# Input Type : tel

Used for telephone numbers.

---

## Syntax

```html
<input
    type="tel">
```

---

## Example

```html
<input
    type="tel"
    id="phone"
    name="phone">
```

---

## Why not number?

Phone numbers

- May contain `+`
- May begin with `0`
- Are identifiers, not values for calculations

Therefore

```html
type="tel"
```

is the correct choice.

---

# Input Type : url

Used for website links.

---

## Syntax

```html
<input
    type="url">
```

---

## Example

```html
<input
    type="url"
    id="portfolio"
    name="portfolio">
```

Valid

```
https://portfolio.com
```

Invalid

```
portfolio
```

The browser validates the format.

---

# Quick Comparison

| Input Type | Purpose |
|------------|---------|
| text | General text |
| email | Email address |
| password | Password |
| number | Numeric values |
| tel | Phone number |
| url | Website URL |

---

# Common Mistakes

❌

```html
<input
    type="number"
    placeholder="Phone Number">
```

✔

```html
<input
    type="tel">
```

---

❌

Using placeholder instead of label.

✔

Always use

```html
<label>

<input>
```

---

❌

Using `disabled` when data must be submitted.

✔

Use `readonly`.

---

# Interview Questions

1. What is a Boolean attribute?
2. Explain `required`.
3. Difference between `readonly` and `disabled`.
4. Is the value of a disabled field submitted?
5. What does `autocomplete` do?
6. What is `autofocus`?
7. Difference between `text` and `email`.
8. Difference between `number` and `tel`.
9. Does `password` encrypt data?
10. What is `type="url"` used for?

---

---

# Progress

```
Day 2 Progress

████████████████░░░░░░░ 75%
```

Completed

- Tables ✅
- Forms Basics ✅
- Form Attributes ✅
- Input Types (Part 1) ✅
