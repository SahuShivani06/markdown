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
### What is specificity?

Specificity in CSS (Cascading Style Sheets) is a set of rules that the browser uses to determine which CSS rule should be applied when multiple rules could apply to the same element.

 Think of it like this:<br>
When more than one rule targets the same element, the browser chooses the one with higher specificity.

Specificity Hierarchy:<br>
From lowest to highest:

Element selector (e.g. div, p, h1) → 1 point

Class selector (e.g. .box, .active) → 10 points

ID selector (e.g. #header, #main) → 100 points

Inline styles (e.g. style="color:red") → 1000 points

!important → Overrides all but should be avoided if possible<hr>

example:<br>
` div {
  color: blue;         /* specificity: 1 */
}
.box {
  color: green;        /* specificity: 10 */
}
#header {
  color: red;          /* specificity: 100 */
} `

The color will be red because #header (100) has the highest specificity.

 Quick Tip:<br>
If two selectors have equal specificity, the one that appears last in the CSS wins.<hr>

 What is Responsiveness in Web Design?<br>
Responsiveness means a website or app adapts its layout and design to look good and work well on all screen sizes — from big desktop monitors to small mobile phones.

 Tools That Help With Responsiveness:<br>
Flexbox – Align and space elements easily

CSS Grid – More powerful layout control

Media Queries – Customize styles for different screen widths

Frameworks – Like Bootstrap or Tailwind CSS<hr>

### What are Media Queries in CSS?
Media queries allow you to change the layout based on the screen size, resolution, orientation, or other device features.

| Feature                     | Meaning                                                 |
| --------------------------- | ------------------------------------------------------- |
| `max-width`                 | Apply when screen is **less than or equal to** value    |
| `min-width`                 | Apply when screen is **greater than or equal to** value |
| `max-height` / `min-height` | Based on screen height                                  |
| `orientation`               | `portrait` or `landscape`                               |
| `prefers-color-scheme`      | Detect light/dark mode                                  |
<hr>
Pro Tip:
You can use breakpoints like:

max-width: 480px → mobile phones

max-width: 768px → tablets

max-width: 1024px → small laptops

min-width: 1025px → desktops<hr>

code

`Default desktop style <br>
.container {<br>
  flex-direction: row;<br>
}

Mobile layout: stack elements vertically <br>
@media (max-width: 768px) {<br>
  .container {<br>
    flex-direction: column;<br>
  }<br>
}`<hr>

What is the Mobile-First Approach in Web Design?<br>
Mobile-first means you start designing and coding your website for small screens (like mobile phones) first, and then add styles for larger screens using media queries.

This approach ensures that your site works perfectly on mobile (which most users use!), and then enhances the layout for tablets and desktops.<hr>

#### Why Use Mobile-First?<br>
Most users browse on phones 📲

Forces you to focus on core content

Improves performance and speed

Recommended by Google for SEO<hr>

 How to Write Mobile-First CSS:

 Write base styles for mobile screens first

Use min-width media queries to add styles for larger screens<hr>

code

`/* 👶 Base: Mobile styles */
.container {
  flex-direction: column;
  font-size: 14px;
}
/* 💻 Tablets and up (>=768px) */
@media (min-width: 768px) {
  .container {
    flex-direction: row;
    font-size: 16px;
  }
}
/* 🖥️ Desktops and up (>=1024px) */
@media (min-width: 1024px) {
  .container {
    font-size: 18px;
  }
}`<hr>

#### What are Pseudo-classes in CSS?<br>
Pseudo-classes are keywords in CSS that let you style elements based on their state, position, or interaction — without needing extra classes or JavaScript.

They are always written with a colon (:) before the keyword.

 Commonly Used Pseudo-classes:<br>

🔹 :hover
Triggered when the user hovers the mouse over an element.

code<br>
`button:hover {
  background-color: green;
  color: white;
}`<br>
👉 Often used for buttons, links, and interactive UI.

🔹 :focus<br>
Activated when an element (like an input box) is focused — e.g., when clicked or selected via keyboard.

`input:focus {
  border: 2px solid blue;
  outline: none;
}`<br>
👉 Great for forms and improving accessibility.

🔹 :nth-child(n)<br>
Targets an element based on its position among siblings.

`li:nth-child(2) {
  color: red;
}`<br>
👉 Changes the 2nd <li> in a list.

You can also use:

:nth-child(odd) → 1st, 3rd, 5th...

:nth-child(even) → 2nd, 4th, 6th...

:nth-child(3n) → every 3rd element (3rd, 6th, 9th...)

Why Use Pseudo-classes?<br>

Add interactivity (:hover, :focus)

Target specific elements without classes (:nth-child)

Write cleaner, shorter CSS<hr>


 ### CSS Colors and Backgrounds<br>
Colors and backgrounds are essential in web design to make your site visually appealing and easy to read.

 Backgrounds<br>
Used to style the background of an element.

🔹 background-color

`div {
  background-color: #f0f0f0;
}`

🔹 background-image

`div {
  background-image: url("image.jpg");
}`

🔹 background-repeat

background-repeat: no-repeat;

Options: repeat, no-repeat, repeat-x, repeat-y

🔹 background-size

`background-size: cover;    
background-size: contain;`

🔹 background-position

`background-position: center;`

🔹 background-attachment

`background-attachment: fixed;`

Stays fixed when scrolling

🎯 Shorthand Example:

`div {
  background: url("bg.jpg") no-repeat center/cover;
}`

This sets:

Image

No repeat

Centered

Cover entire element
<hr>
What is RGB in CSS?

RGB stands for Red, Green, Blue — it’s a color model used in CSS (and in computers in general) to create any color by mixing different intensities of red, green, and blue light.


| Color | RGB Code             | Output                    |
| ----- | -------------------- | ------------------------- |
| Red   | `rgb(255, 0, 0)`     | 🔴 Full red               |
| Green | `rgb(0, 255, 0)`     | 🟢 Full green             |
| Blue  | `rgb(0, 0, 255)`     | 🔵 Full blue              |
| Black | `rgb(0, 0, 0)`       | ⚫ No color = black        |
| White | `rgb(255, 255, 255)` | ⚪ All colors full = white |
| Gray  | `rgb(128, 128, 128)` | 🟤 Balanced mix           |

🧠 RGB Format:

color: rgb(red, green, blue);

Each value:

R (Red), G (Green), B (Blue)

Ranges from 0 to 255

0 means none of that color

255 means full intensity

You Can Also Use RGBA:

a stands for Alpha (transparency)


color: rgba(255, 0, 0, 0.5);  /* Red with 50% transparency */

🎯 When to Use RGB?

When you want precise control over color tones

When using JavaScript to change colors dynamically

When adding transparency with rgba<hr>

You Can Also Use RGBA:

a stands for Alpha (transparency)

color: rgba(255, 0, 0, 0.5);  /* Red with 50% transparency */<hr>

🎯 When to Use RGB?

When you want precise control over color tones

When using JavaScript to change colors dynamically

When adding transparency with rgba
<hr>

 ### What is position in CSS?
The position property tells where and how an element should appear on the page.
There are 5 main types of positioning:

1. 🟢 static (Default Position)

This is the normal/default position.

The element appears where it normally would on the page.

You can’t move it using top, left, right, or bottom.

🔹 Example:

You write text in a notebook. Each line follows the one above it.

That’s how elements behave with static — just stack up one after the other.

`div {
  position: static;
}`<hr>

2. 🟡 relative

The element stays in its normal place, BUT…

You can now use top, left, right, or bottom to move it slightly.

It still takes up the original space.

🔹 Example:

Imagine a photo frame on a wall. You shift it a little to the right or down.

It’s still in its place, just nudged.

`div {
  position: relative;
  top: 20px;
  left: 30px;
}`

✅ Moves, but doesn’t affect the layout of other elements.<hr>


3. 🔴 absolute

The element is completely removed from the normal flow.

It is placed based on the nearest positioned parent (not static).

If there’s no such parent, it uses the whole page as reference.

🔹 Example:

Imagine sticking a sticky note on a photo frame.

Wherever the frame goes, the sticky note sticks based on the frame.

`.parent {
  position: relative;
}
.child {
  position: absolute;
  top: 0;
  right: 0;
}`

✅ Useful for popups, tooltips, modals, badges.<hr>

4. 🔵 fixed

The element is fixed to the screen, not the page.

It doesn't move even when you scroll.

It stays where you place it on the viewport (screen).

🔹 Example:

A sticky button in a mobile app that stays in the corner as you scroll.

`div {
  position: fixed;
  bottom: 10px;
  right: 10px;
}`

✅ Great for headers, footers, back-to-top buttons.<hr>

5. 🟣 sticky

This is a mix of relative and fixed.

It acts like relative at first…

But when you scroll down, it "sticks" to a certain spot (like the top of the screen).

🔹 Example:

A menu bar that scrolls with the page, but sticks to the top when it reaches it.

`div {
  position: sticky;
  top: 0;
}`

✅ Very useful for sticky navigation bars.
