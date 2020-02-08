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

Correct
```html
<ul>
  <li>Rocky road </li>
  <li>Strawberry</li>
</ul>
```

Incorrect
```html
<ul>
  <li>Rocky road </li>
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
<img src="/slides/img/code.jpg" width=300px />
```

* ``src`` - location of the image file
* Demo get an image from the internet
-

## Links - Inline

A is for `anchor`

```html
<a href="http://youtube.com">Youtube</a>
```

* ``href`` - short for hyperlink reference.

* <a href="http://youtube.com">Youtube</a>

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

<img src="http://2.bp.blogspot.com/_UjJgEwVlPQs/Sxg-OdZMD0I/AAAAAAAADlg/gkTWJLBTaOM/s1600/Golden_Retriever_Puppies.jpg" width="800px">

-
-
## CSS

-

## Anatomy of a website

* HTML - content (what it has)
* CSS - presentation (how it looks)

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
## Selector: Class

```html
<h1 class="main-title">My website</h1>
<h1>Lisa's website</h1>
```

Select the class name with a `.`

```
.main-title {
  background-color: blue;
}
```

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

## Size

```
p {
  width: 50%;
  height: 300px;
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
<img src="http://cdn7.whiskeyriff.com/wp-content/uploads/cutest-puppy-ever-1384460985_org.jpg">
