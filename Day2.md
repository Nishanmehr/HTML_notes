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




# 📅 Day 2 - HTML Forms (Part 2)

---

# 📌 More Input Types

HTML provides many input types for different kinds of user data.

---

## 1. Date (`type="date"`)

### Definition

Used to select a calendar date.

### Syntax

```html
<label for="dob">Date of Birth</label>
<input type="date" id="dob" name="dob">
```

---

## 2. Time (`type="time"`)

### Definition

Used to select only time.

### Syntax

```html
<label for="time">Meeting Time</label>
<input type="time" id="time" name="time">
```

---

## 3. Datetime Local (`type="datetime-local"`)

### Definition

Used to select both date and time together.

### Syntax

```html
<label for="interview">Interview Time</label>
<input
type="datetime-local"
id="interview"
name="interview">
```

---

## 4. Month (`type="month"`)

### Definition

Allows the user to select only a month and year.

### Syntax

```html
<label for="month">Joining Month</label>
<input
type="month"
id="month"
name="month">
```

---

## 5. Week (`type="week"`)

### Definition

Allows the user to select a specific week of a year.

### Syntax

```html
<label for="week">Select Week</label>
<input
type="week"
id="week"
name="week">
```

---

## 6. Color (`type="color"`)

### Definition

Displays a color picker.

### Syntax

```html
<label for="color">Favorite Color</label>
<input
type="color"
id="color"
name="color">
```

---

## 7. Range (`type="range"`)

### Definition

Creates a slider.

### Syntax

```html
<label for="rating">Rating</label>

<input
type="range"
id="rating"
name="rating"
min="0"
max="10">
```

---

## 8. Search (`type="search"`)

### Definition

Used for search fields.

### Syntax

```html
<label for="search">Search</label>

<input
type="search"
id="search"
name="search"
placeholder="Search here...">
```

---

## 9. File (`type="file"`)

### Definition

Used to upload files.

### Syntax

```html
<label for="resume">Upload Resume</label>

<input
type="file"
id="resume"
name="resume">
```

### Multiple Files

```html
<input
type="file"
multiple>
```

---

## 10. Hidden (`type="hidden"`)

### Definition

Stores hidden information that users cannot see.

### Syntax

```html
<input
type="hidden"
name="employeeId"
value="EMP1001">
```

---

# 📌 Selection Controls

---

# Radio Button

## Definition

Allows selecting only one option.

### Syntax

```html
<label for="male">Male</label>
<input
type="radio"
id="male"
name="gender"
value="Male">

<label for="female">Female</label>
<input
type="radio"
id="female"
name="gender"
value="Female">

<label for="other">Other</label>
<input
type="radio"
id="other"
name="gender"
value="Other">
```

### Important Points

- Same `name`
- Different `id`
- One option only
- `checked` selects by default

---

# Checkbox

## Definition

Allows selecting multiple options.

### Syntax

```html
<label for="html">HTML</label>
<input
type="checkbox"
id="html"
name="skills"
value="HTML">

<label for="css">CSS</label>
<input
type="checkbox"
id="css"
name="skills"
value="CSS">
```

### Important Points

- Multiple selections
- Unique IDs
- Can use same `name`
- `checked` selects by default

---

# 📌 Dropdown

## `<select>`

Creates a dropdown.

```html
<select id="role" name="role">

<option value="">Select Role</option>

<option value="developer">
Developer
</option>

<option value="tester">
Tester
</option>

</select>
```

---

## `<option>`

Represents one item inside a dropdown.

```html
<option value="java">
Java Developer
</option>
```

---

## `<optgroup>`

Groups options together.

```html
<select>

<optgroup label="North India">

<option>Delhi</option>

<option>Noida</option>

</optgroup>

<optgroup label="South India">

<option>Bangalore</option>

<option>Hyderabad</option>

</optgroup>

</select>
```

---

# 📌 Textarea

## Definition

Used for multi-line text input.

```html
<textarea
rows="5"
cols="40"
placeholder="Tell us about yourself">
</textarea>
```

---

# 📌 Buttons

## Submit

```html
<button type="submit">
Submit
</button>
```

Submits the form.

---

## Reset

```html
<button type="reset">
Reset
</button>
```

Resets the form.

---

## Button

```html
<button type="button">
Click Me
</button>
```

Used with JavaScript.

---

# 📌 HTML5 Validation

## `min`

```html
<input
type="number"
min="18">
```

Minimum allowed value.

---

## `max`

```html
<input
type="number"
max="60">
```

Maximum allowed value.

---

## `minlength`

```html
<input
type="text"
minlength="3">
```

Minimum number of characters.

---

## `maxlength`

```html
<input
type="text"
maxlength="30">
```

Maximum number of characters.

---

## `pattern`

```html
<input
type="password"
pattern=".{8,}">
```

Custom validation using Regular Expressions.

---

## `step`

```html
<input
type="number"
step="1">
```

Controls increment values.

---

## `multiple`

```html
<input
type="file"
multiple>
```

Allows selecting multiple files.

---

# 📊 Interview Differences

## Radio vs Checkbox

| Radio | Checkbox |
|--------|----------|
| One option | Multiple options |
| Same `name` | Independent |
| Gender | Skills |

---

## Readonly vs Disabled

| Readonly | Disabled |
|-----------|----------|
| Cannot edit | Cannot edit |
| Value submitted | Value not submitted |
| Can copy | Cannot interact |

---

## Placeholder vs Value

| Placeholder | Value |
|-------------|-------|
| Hint | Default value |
| Not submitted | Submitted |
| Disappears | Remains |

---

## ID vs Name

| ID | Name |
|----|------|
| Unique | Can repeat |
| Used by label | Used to send data |
| CSS & JavaScript | Server |

---

# 🎯 Common Interview Questions

1. What is an HTML Form?
2. Difference between GET and POST.
3. Difference between `id` and `name`.
4. Difference between `readonly` and `disabled`.
5. Difference between radio and checkbox.
6. Difference between `placeholder` and `value`.
7. Difference between `<input>` and `<textarea>`.
8. What is `<select>`?
9. What is `<option>`?
10. What is `<optgroup>`?
11. What is `<textarea>`?
12. What are the types of buttons?
13. What is the default type of `<button>`?
14. What is `min`?
15. What is `max`?
16. What is `minlength`?
17. What is `maxlength`?
18. What is `step`?
19. What is `multiple`?
20. What is `pattern`?

---

# ✅ Day 2 Completed

## Topics Covered

- Forms
- Form Attributes
- Labels
- Input Types
- Date
- Time
- Datetime-local
- Month
- Week
- Color
- Range
- Search
- File
- Hidden
- Radio Button
- Checkbox
- Dropdown
- Select
- Option
- Optgroup
- Textarea
- Buttons
- HTML5 Validation
- Interview Questions

---

## 📈 Progress

```text
Day 1 ✅ Completed
Day 2 ✅ Completed

Overall HTML Progress

█████████████████████████ 95%
```

