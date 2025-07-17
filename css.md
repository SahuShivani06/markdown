## What Is a Selector?
A selector targets HTML elements so you can style them using CSS.

There are 3 essential types you must learn first:
1. Element Selector<br>
🎯 Targets all HTML elements of a specific type.


` p {
  color: red;
} `

2. Class Selector (.)<br>
🎯 Targets elements with a class attribute. You can use the same class on many elements<br>
`.note {
  color: blue;
}`


3. ID Selector (#)<br>
🎯 Targets an element with a unique ID (should be used only once per page).<br>
`#main-title {
  font-size: 30px;
}`

### Typography

| Property      | Example               |
| ------------- | --------------------- |
| `color`       | `color: red;`         |
| `font-size`   | `font-size: 18px;`    |
| `font-family` | `font-family: Arial;` |
| `text-align`  | `text-align: center;` |
| `font-weight` | `font-weight: bold;`  |

3. Box Model (Spacing & Sizing)
Every HTML element is a box with:<br>
Content<br>
Padding (space inside the box)<br>
Border<br>
Margin (space outside the box)

`div {<br>
  padding: 10px;<br>
  margin: 20px;<br>

border: 2px solid black;<br>
}`<hr>

4. Layout Basics (Display & Positioning)<br>

| Value          | Meaning                                   |
| -------------- | ----------------------------------------- |
| `block`        | Takes full width (e.g., `<div>`)          |
| `inline`       | Fits next to other items (e.g., `<span>`) |
| `inline-block` | Like inline, but allows width/height      |
| `flex`         | For modern layout (flexbox)               |

`.container {
  display: flex;
}`<hr>

What is Responsiveness?<br>
Responsive Design means your website adapts to different screen sizes using flexible layouts, media queries, and percentage-based widths.

1. Flexible Units (%, vw, vh, em, rem)<br>
Use relative units instead of fixed px.

`.container {<br>

width: 80%;      /* relative to parent */<br>
  padding: 2em;    /* relative to font-size */<br>
}`
