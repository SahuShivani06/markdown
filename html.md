# HTML

## HTML boilerplate 
` <!DOCTYPE html > `<br>
`<html lang="en">` <br>
`<head>` <br>
`</head>`<br>
`<body>`<br>
`</body>`<br>
`</html>`<br>

## Common Tags
<h1> Heading 1 </h1>
<h2> Heading 2 </h2>
<h3> Heading 3 </h3>
<h4> Heading 4 </h4>
<h5> Heading 5 </h5>
<h6> Heading 6 </h6><hr>

#### Paragraph tag
<p>This is a paragraph tag</p><hr>

#### link tag
<a href="https://www.google.com"> Google</a><hr>
 
 #### Image tag 
 ![bird](StockSnap_OXW52JDMAI-1.jpg)
 `<img src=![bird](StockSnap_OXW52JDMAI-2.jpg)>`
 <br><hr>

 #### Lists
  
 ` <ul>` = unordered list<br>
 `<ol>` = ordered list<br>
 `<li>`= list item<br>

 Unordered list
 <ul>
  <li>Milk</li>
  <li>Bread</li>
  <li>Eggs</li>
</ul>

Ordered list
<ol>
  <li>Wake up</li>
  <li>Brush teeth</li>
  <li>Go to school</li>
</ol>
<hr>

#### Forms and inputs

| Tag          | Purpose                                                   |
| ------------ | --------------------------------------------------------- |
| `<form>`     | Wraps all form elements and sends data to a server        |
| `<input>`    | A one-line field for text, numbers, email, password, etc. |
| `<button>`   | A clickable button (usually for submitting the form)      |
| `<textarea>` | A multi-line input for longer text (like comments)        |
| `<select>`   | A dropdown menu                                           |
| `<option>`   | Individual items inside a `<select>` dropdown             |

code

<form action="/submit" method="post">
  <label>Name:</label>
  <input type="text" name="username" />

  <br>

  <label>Message:</label>
  <textarea name="message"></textarea>

  <br>

  <label>Gender:</label>
  <select name="gender">
    <option value="male">Male</option>
    <option value="female">Female</option>
  </select>

  <br>

  <button type="submit">Send</button>
</form>
<hr>

#### Semantic Tags

| Tag         | Purpose                                                   |
| ----------- | --------------------------------------------------------- |
| `<header>`  | Top part of the page (logo, title, navigation)            |
| `<nav>`     | Navigation links (menu, links to other pages)             |
| `<main>`    | Main content area of the page                             |
| `<section>` | A section of related content (like a chapter or category) |
| `<article>` | Independent content (like a blog post or news article)    |
| `<footer>`  | Bottom part of the page (contact info, copyright)         |

code

<!DOCTYPE html>
<html>
  <head>
    <title>Semantic HTML Example</title>
  </head>
  <body>
    <header>
      <h1>My Website</h1>
      <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
      </nav>
    </header>

 <main>
      <section>
        <h2>Welcome!</h2>
        <p>This is the homepage of my site.</p>
      </section>

<article>
        <h3>Latest Blog Post</h3>
        <p>This is a blog post about web development.</p>
      </article>
    </main>

<footer>
      <p>© 2025 My Website. All rights reserved.</p>
    </footer>
  </body>
</html><hr>

#### Table

| Tag       | Stands For        | Purpose                                    |
| --------- | ----------------- | ------------------------------------------ |
| `<table>` | Table             | Starts and ends the table                  |
| `<tr>`    | Table Row         | Defines a row in the table                 |
| `<td>`    | Table Data Cell   | Holds data inside a row (normal cells)     |
| `<th>`    | Table Header Cell | Header cell (bold and centered by default) |

code

<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>Shivani</td>
    <td>22</td>
    <td>Mumbai</td>
  </tr>
  <tr>
    <td>sujata</td>
    <td>24</td>
    <td>Pune</td>
  </tr>
</table><hr>

#### Attributes

| Attribute     | Used With               | Purpose / Meaning                                          |
| ------------- | ----------------------- | ---------------------------------------------------------- |
| `href`        | `<a>` (anchor tag)      | Specifies the link URL (used for hyperlinks)               |
| `src`         | `<img>`, `<iframe>`     | Specifies the source of media (like an image)              |
| `alt`         | `<img>`                 | Alt text if image doesn’t load (also helps screen readers) |
| `type`        | `<input>`, `<button>`   | Defines input type (text, password, email, etc.)           |
| `value`       | `<input>`               | Sets the default or submitted value of an input field      |
| `placeholder` | `<input>`, `<textarea>` | Gray text inside input box as a hint                       |

🔸 Examples:
1. href — for links<br>
<a href="https://www.google.com">Go to Google</a><br>
✔ Creates a clickable link.

2. src and alt — for image<br>
<img src="cat.jpg" alt="A cute cat" /><br>
✔ Shows an image; if it can't load, "A cute cat" is shown.

3. type, value, and placeholder — for form input<br>
<input type="text" placeholder="Enter your name" value="Shivani" /><br>
✔ Input box for name with a hint and pre-filled value.
