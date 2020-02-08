# Intro to HTML & CSS
-
-

## HTML

-
-

## What is HTML?

HTML is the code for creating web pages.

<img src="/slides/img/youtube.jpg">

* Stands for `Hyper Text Markup Language`

-
## Example of HTML

```
<h1>Intro to HTML</h1>
```

```
<p>talk about html</p>
```

```
<h3>Favorite ice cream</li>
<ul>
  <li>Rocky road </li>
  <li>chocolate</li>
  <li>Strawberry</li>
</ul>
```

-

## HTML Element

<img src="/slides/img/html-element.png" />

* Tag Name/Type
* Opening Tag
* Closing Tag
* Content

-

## Empty Elements

Some elements do not have content, so they are self closing.

```html
<img src="/slides/img/code.jpg" />
```

<img src="/slides/img/code.jpg">

-

## HTML Attribute

Provides additional information about the HTML element

<img src="/slides/img/html-attribute.png" />

`class` is the attribute name

 `editor-note` is the value

-
## Example of HTML Attribute

```
<img id="apple-pic" class="profile-pic" src="apple.jpg" height=300px />
```

- id
- class
- width
- height

-
-

## Nesting elements

You can place HTML elements inside other elements.

Mind your opening and closing tags.

Correct
```html
<ul>
  <li>Rocky road </li>
  <li>chocolate</li>
  <li>Strawberry</li>
</ul>
```

Incorrect
```html
<ul>
  <li>Rocky road </li>
  <li>chocolate</li>
  <li>Strawberry
  </ul>
</li>
```
-

## HTML document
A text file of web page content wrapped in HTML tags.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image">
  </body>
</html>

```

-
-

## Basic HTML Elements

-

## Headings - Block Level

Mark content as heading. HTML has 6 levels.

```html
<h1>My main title</h1>
<h2>My top level heading</h2>
<h3>My subheading</h3>
<h4>My sub-subheading</h4>
```

<h1>My main title</h1>
<h2>My top level heading</h2>
<h3>My subheading</h3>
<h4>My sub-subheading</h4>
-

## Paragraphs - Block Level

Paragraphs of text.

```html
<p>This is a single paragraph</p>
```

<p>This is a single paragraph</p>

-

## Lists - Block Level

Unordered list is used to described a list with no order.

By default, they are bullet points.


```html
<ul>
    <li>Cookies</li>
    <li>Ice-cream</li>
    <li>Fruits</li>
</ul>
```
<ul>
    <li>Cookies</li>
    <li>Ice-cream</li>
    <li>Fruits</li>
</ul>

-

## Images - Inline

<img src="/slides/img/code.jpg" width=100px />

```html
<img src="/slides/img/code.jpg" width=100px />
```

* ``src`` - location of the image file

-

## Links - Inline

A is for `anchor`

```html
<a href="http://youtube.com">Youtube</a>
```

``href`` - short for hyperlink reference.

<a href="http://youtube.com">Youtube</a>

-
## Line/Ruler

```
<hr />
```
<hr />

-
## Line break
HTML ignores white space and new  line in the document.

### Line break
```
<br \>
```

a<br>b

-

## Span - Inline

When you need to add inline style and you can't think of a better tag, use span.

```
<p>this is <span style="color:red">red</span></p>
```

<p>this is <span style="color:red">red</span></p>

-

## HTML5 Components

* `<header>` - top content (e.g. title, logo, or navigation)
* `<nav>` - navigation
* `<main>` - content
* `<footer` - bottom content (e.g. contact info, copyright, sub navigation)

-

## Div - Block

When you need to wrap elements and can't think of a better tag.

```html
<div class="shopping-cart">
  <h2>Shopping cart</h2>
      <p><a href="">Cashmere sweater</a>: $99.95.</p>
      <img src="/slides/img/cash.png" alt="Cashmere sweater">
  <p>Total cost: $237.89</p>
</div>
```
-
-

## HTML Resources
- [MDN HTML API](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [Khan academy](https://www.khanacademy.org/computing/computer-programming/html-css)
- [Common Tags](http://www.washington.edu/accesscomputing/webd2/student/unit2/common_tags.html)
- [FreeCodeCamp](https://www.freecodecamp.org)
- [HTML & CSS Book](http://htmlandcssbook.com/code-samples/chapter-01/)

-
-

<img src="http://2.bp.blogspot.com/_UjJgEwVlPQs/Sxg-OdZMD0I/AAAAAAAADlg/gkTWJLBTaOM/s1600/Golden_Retriever_Puppies.jpg" width="800px">

-
-
## CSS

-

## Anatomy of a website

* HTML - content
* CSS - presentation

-
## What is CSS?

CSS stands for Cascading Style Sheets.

It adds styles to the content (HTML).

It makes your webpage looks pretty.

```CSS
header {
    background-color: teal;
    height: 160px;
}

header p {
  background-color: green;
}
```

-

## What is a CSS rule?

<img src="/slides/img/cssrule.png">

-
-
## Selector: Element

```
p {
  background-color: blue;
}
```

Selects all paragraph elements.

```
img {
  width: 100px;
}
```

Selects all image elements.

-
## Selector: Position

```
p em {
  color: yellow;
}
```

Selects all `em` elements that are within a paragraph

```
<p>This is <em>important.</em></p>
```

<p>This is <em style="color:yellow">important.</em></p>

-
## Selector: Position
- Position selectors are more specific
- They look for elements inside other elements
- We separate nested elements with a space
- Position selectors will override general selector

```
header ul {
  <!-- text in header ul is red (except if it's a link) -->
  color: red;
}

ul {
   <!-- all text in a list is green (except header list) -->
  color: green;
}

ul li a{
  <!-- link text is purple -->
  color: purple;
}
```

-
-

## CSS Color Values

Your browser can accept colors in many different ways:

- Hexadecimal value (ex. #FF0000)
- RGB value (ex. rgb(255, 0, 0))
- HSL value (ex. hsl(0, 100%, 100%))
- Color name (ex. red)
  - The 17 standard colors are: aqua, black, blue, fuchsia, gray, grey, green, lime, maroon, navy, olive, purple, red, silver, teal, white, and yellow.

-
## Color

The `color` property changes the color of the text.

Hexadecimal (most common)

```
p {
  color: #ff0000;
}
```

RGB values

```
p {
  color: rgb(255, 0, 0);
}
```

Color name

```
p {
  color: red;
}
```

-

## Background

```
p {
  <!-- set background color -->
  background-color: #81D8D4;

  <!-- set background image. This will override color -->
  background-image: url('img/castle.jpg');

  <!-- does not move -->
  background-position: fixed;

  <!-- repeats vertically -->
  background-repeat: repeat-y;
}
```

```
p {
  <!-- set everything in one line -->
  background: #81D8D4 url('img/castle.jpg') fixed repeat-y;
}
```

<p style="background-color:#81D8D4">this is a paragraph with background</p>

[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/background)

-

## Font

```
p {
  font-family: "Arial", sans-serif;
  font-size: 16px;
  font-weight: bold;
  font-style: italic;
}
```

```
p {
  <!-- set everything in one line -->
  font: bold italic 16px "Arial", sans-serif;
}
```
-

## Font-size
The font-size property specifies the size of the font.

```
p {
  <!-- Pixels -->
  font-size: 12px;

  <!-- em - 150% more than the inherited size  -->
  font-size: 1.5em;

  <!-- percent - 150% more than the inherited size -->
  font-size: 150%;
}
```

[W3 school](https://www.w3schools.com/cssref/tryit.asp?filename=trycss_font)
-

## Font properties

```
p {
  text-align: center;
  line-height: 16px;
  vertical-align: super;
  letter-spacing: 10px;
}
```

[W3 school](https://www.w3schools.com/cssref/pr_pos_vertical-align.asp)

-
## List

```
ul {
  list-style: square url("sqpurple.gif");
}

```
-
-

## Spacing

<img src="https://pressupinc.com/wp-content/uploads/2014/01/box-model.png">

- padding
- border
- margin

-

## Padding

The space between the content and its border. [W3 School](https://www.w3schools.com/cssref/pr_padding.asp)

```
p {
  padding-top: 10px;
  padding-right: 5px;
  padding-bottom: 30px;
  padding-left: 20px;
}
```

```
p {
  <!-- top, right, bottom, left -->
  padding: 10px 5px 30px 20px;
}
```

```
p {
  <!-- top & bottom is 10px, left & right is 20px -->
  padding: 10px 20px;
}
```

```
p {
  <!-- everything is 10px -->
  padding: 10px;
}
```

-

## Border

```
p {
  border: solid 1px #00ff00;
}

```

```
p {
  border-top: solid 1px #0f0;
  border-bottom: solid 1px #f00;
  border-left: solid 1px #00f;
  border-right: solid 1px #000;
}

```

<p style="border: solid 1px #00ff00;">Border</p>

-

## Margin

```
p {
  margin: solid 1px #00ff00;
}

```

```
p {
  margin-top: solid 1px #0f0;
  margin-bottom: solid 1px #f00;
  margin-left: solid 1px #00f;
  margin-right: solid 1px #000;
}

```
-
## Spacing

<img src="https://pressupinc.com/wp-content/uploads/2014/01/box-model.png">

-
-
## Position

```
p {
  position: fixed;
  top: 40px;
  right: 100px;
}
```

- fixed - starts from the top left document
- relative - relative to other documents

[MDN Position](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
-

## Size

```
p {
  width: 50%;
  height: 300px;
}
```

-
-

## CSS selectors : Tag

You can select elements by their html tag name.

```CSS
/* Targets the <h1> element */
h1 {
    color: pink;
    font-size: 22px;
}

/* Targets the <header> element */
header {
    height: 160px;
    background-color: blue;
}
```
-

## Multi Selectors

Applies a single CSS rule set to multiple selectors. Each selector is separated by a comma.

```CSS
h1,
h2,
h3,
h4 {
    color: pink;
    font-size: 22px;
}
```

-

## Descendant Selector

Specifically targets any h1 that is a descendant (or nested within) a header

```CSS
header h1 {
    font-size: 60px;
}

h1 {
    font-size: 32px;
}
```

-

## Child Selector

Specifically targets direct child of tag `p` of type `<a>`

```CSS
p > a {
  color: red;
}
```

- [Google](http://google.com)

<p>this is a paragraph with link to <a href="http://yahoo.com" style="color:red">Yahoo</a><p>


-

## Sibling Selector

Specifically targets any h1 that is a descendant (or nested within) a header

```CSS
li+li {
  color: red;
}
```

<ul>
  <li>Chapter 1</li>
  <li style="color:red">Chapter 2</li>
  <li style="color:red">Chapter 3</li>
</ul>

-
## Id selector

```
<p id="bio">This is bio</p>
<p>nothing to see here</p>
```

```
#bio {
  color:red;
}
```

<p style="color:red">This is bio</p>
<p>nothing to see here</p>


-

## Class selector

```
<button class="primary">Submit</button>
<button>Next</button>
```

```
.primary {
  color:red;
}
```

<button style="color:red; font-size:30px">Submit</button>
<button style="font-size:30px">Next</button>

-

## Class child selector

```
.bio .header {
    font-size: 60px;
}

```

```
<h2 class="header">Bio</h2>

<div class="bio">
  <!--  this header font size is 60px -->
  <h2 class="header">Early years</h2>

</div>
```
-

## Attribute selector

```html
<label for="username">Username</label>
<input id="username" type="text" />
<br>
<label for="icecream">Love ice-cream?</label>
<input id="icecream" type="checkbox" />

```

Select by attribute

```
[type="checkbox"] {
 font-size:40px;
}
```

Select by tag with a given attribute

```
input[type="checkbox"] {
 font-size:40px;
}
```

-
-

## Inherit

Children inherit attributes from their parents

```
body {
  font: "Arial";
}

header {
  font: "Times"
}
```

-
## Inherit Property

```
/* Make second-level headers green */
h2 { color: green; }

/* header in sidebar will inherit from the parent class */
#sidebar h2 { color: inherit; }
```

-

## Inherit

- All browser have some type of defaults
- Designer usually `normalize` (reset) all the elements so left 10px means left 10px everywhere

-
-
## Cascading
Styles "cascade" down until changed

```
p{
  color:blue;
  font-family: 'Helvetica';
}
.red {
  color: red;
}
#special {
  font-family: Arial;
}
```

```
<p>Paragraph</p>
<p class ="red">Paragraph</p>
<p class = "red" id ="special">Paragraph</p>
```

-

## Cascading priority
Your browser assigns different priorities to CSS depending on the type of selector.

1. Important! - Most Important
2. In line CSS
3. ID
4. Class
5. Element - Least Important

-

## Cascading priority
Your browser also assigns priority based on the specificity of the selection. More specific selectors have higher priority.

```
.main .sale .clearance p{ //Most specific
  color: red;
}
.header .title p{
  color: green;
}
.footer p{ //Least specific
  color: blue;
}
```

-
-

## Connecting CSS to HTML
- "External"
- "Inline"
- "Embedded"

-

## External

Preferred style

style.css

```CSS
h1 {
  color: pink;
}
```

index.html

```html
<html>
  <head>
    <link rel="stylesheet" href="/style.css">
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```

-

## Inline

```
<p style="color:red">Some text.</p>
```

Applies to specific element

Can't be reused

DON'T DO IT!

(unless you really really have to)

-
## Embedded
```
<head>
  <style type="text/css">
    p {
      color: red;
      font-size: 12px;
    }
  </style>
</head>
```

Inside <head> of the HTML document.

Uses `<style>` tag.

Can only be used in one HTML file
-
-

## Demo
- view CSS property of an element in the browser
- modify property

-
## Resources
 - [MDN CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
 - [W3schools CSS](https://www.w3schools.com/cssref/default.asp)

-
<img src="http://cdn7.whiskeyriff.com/wp-content/uploads/cutest-puppy-ever-1384460985_org.jpg">
