---
istop: true
title: Bootstrap 4 Get Started
date: 2017-10-27 11:09:00
background-image: ../style/images/bootstrap-4.jpeg
category: bootstrap
tags: bootstrap frontend
---
## Resources
[Bootstrap 4 class reference](https://hackerthemes.com/bootstrap-cheatsheet/#!)
## Bootstrap 4 CDNvn
If you don't want to download and host Bootstrap 4 yourself, you can include it from a CDN (Content Delivery Network).

MaxCDN provides CDN support for Bootstrap's CSS and JavaScript. You must also include jQuery:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap 4 Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- Latest compiled and minified CSS -->
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css">
  <!-- jQuery library -->
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
  <!-- Popper JS -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.6/umd/popper.min.js"></script>
  <!-- Latest compiled JavaScript -->
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/js/bootstrap.min.js"></script>
</head>
<body>

<div class="container">
  <h1>My First Bootstrap Page</h1>
  <p>This is some text.</p>
</div>

</body>
</html>
```

## 3. Containers
Bootstrap 4 also requires a containing element to wrap site contents.

There are two container classes to choose from:
1. The .container class provides a responsive fixed width container
2. The .container-fluidd class provides a full width container, spanning the entire width of the viewport

## Grid Basic
Bootstrap 4 uses a mobile-first flexbox grid system allows up to 12 columns across the page.

If you do not want to use all 12 columns individually, you can group the columns together to create wider columns:
### grid classes
* .col- (extra small devices - screen width equal to or less than 576px)
* .col-sm- (small devices - screen width equal to or greater than 576px)
* .col-md- (medium devices - screen width equal to or greater than 768px)
* .col-lg- (large devices - screen width equal to or greater than 992px)
* .col-xl- (xlarge devices - screen width equal to or greater than 1200px)
### basic structure of grid
```html
<!-- Control the column width, and how they should appear on different devices -->
<div class="row">
  <div class="col-sm-4"></div>
  <div class="col-sm-12"></div>
</div>

<!-- Or let Bootstrap automatically handle the layout, each cols are equal width -->
<div class="row">
  <div class="col"></div>
  <div class="col"></div>
  <div class="col"></div>
</div>
```
## Typographical
### Display Headings
Display headings are used to stand out more than normal headings (larger font-size and lighter font-weight), and there are four classes to choose from: .display-1, .display-2, .display-3, .display-4
```html
<div class="container">
  <h1>Display Headings</h1>
  <p>Display headings are used to stand out more than normal headings (larger font-size and lighter font-weight):</p>
  <h1 class="display-1">Display 1</h1>
  <h1 class="display-2">Display 2</h1>
  <h1 class="display-3">Display 3</h1>
  <h1 class="display-4">Display 4</h1>
</div>
```
### \<small\>
In Bootstrap 4 the HTML <small> element is used to create a lighter, secondary text in any heading:
```html
<div class="container">
  <h1>Lighter, Secondary Text</h1>
  <p>The small element is used to create a lighter, secondary text in any heading:</p>       
  <h1>h1 heading <small>secondary text</small></h1>
  <h2>h2 heading <small>secondary text</small></h2>
</div>
```
### \<mark\>
Bootstrap 4 will style the HTML <mark> element with a yellow background color and some padding:

```html
<div class="container">
  <h1>Highlight Text</h1>    
  <p>Use the mark element to <mark>highlight</mark> text.</p>
</div>
```
### \<abbr\>
Bootstrap 4 will style the HTML <abbr> element with a dotted border bottom:
```html
<div class="container">
  <h1>Abbreviations</h1>
  <p>The abbr element is used to mark up an abbreviation or acronym:</p>
  <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
</div>
```
### \<blockquote\>
Add the .blockquote class to a <blockquote> when quoting blocks of content from another source:
```html
<div class="container">
  <h1>Blockquotes</h1>
  <p>The blockquote element is used to present content from another source:</p>
  <blockquote class="blockquote">
    <p>For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.</p>
    <footer class="blockquote-footer">From WWF's website</footer>
  </blockquote>
</div>
```
### \<dl\>
Bootstrap 4 will style the HTML <dl> element in the following way:
```html
<div class="container">
  <h1>Description Lists</h1>    
  <p>The dl element indicates a description list:</p>
  <dl>
    <dt>Coffee</dt>
    <dd>- black hot drink</dd>
    <dt>Milk</dt>
    <dd>- white cold drink</dd>
  </dl>     
</div>
```
### <code>
Bootstrap 4 will style the HTML <code> element in the following wa
```html
<div class="container">
  <h1>Code Snippets</h1>
  <p>Inline snippets of code should be embedded in the code element:</p>
  <p>The following HTML elements: <code>span</code>, <code>section</code>, and <code>div</code> defines a section in a document.</p>
</div>
```
### \<kbd\>
Bootstrap 4 will style the HTML \<kbd\> element in the following way:
```html
<div class="container">
  <h1>Keyboard Inputs</h1>
  <p>To indicate input that is typically entered via the keyboard, use the kbd element:</p>
  <p>Use <kbd>ctrl + p</kbd> to open the Print dialog box.</p>
</div>
```
<div class="container">
  <h1>Keyboard Inputs</h1>
  <p>To indicate input that is typically entered via the keyboard, use the kbd element:</p>
  <p>Use <kbd>ctrl + p</kbd> to open the Print dialog box.</p>
</div>
### \<pre\>
```html
<div class="container">
<h1>Multiple Code Lines</h1>
<p>For multiple lines of code, use the pre element:</p>
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks.
</pre>
</div>
```

class                 | description
----------------------|--------------
.font-weight-bold     |	Bold text	Try it
.font-weight-normal   |	Normal text	Try it
.font-weight-light    | Light weight text	Try it
.font-italic	        | Italic text	Try it
.lead	                | Makes a paragraph stand out	Try it
.small	              | Indicates smaller text (set to 85% of the size of the parent)	Try it
.text-left	          | Indicates left-aligned text	Try it
.text-center	        | Indicates center-aligned text	Try it
.text-right	          | Indicates right-aligned text	Try it
.text-justify	        | Indicates justified text	Try it
.text-nowrap	        | Indicates no wrap text	Try it
.text-lowercase	      | Indicates lowercased text	Try it
.text-uppercase	      | Indicates uppercased text	Try it
.text-capitalize	    | Indicates capitalized text	Try it
.initialism	          | Displays the text inside an <abbr> element in a slightly smaller font size	Try it
.list-unstyled	      | Removes the default list-style and left margin on list items (works on both <ul> and <ol>). This class only applies to immediate children list items (to remove the default list-style from any nested lists, apply this class to any nested lists as well)	Try it
.list-inline	        | Places all list items on a single line (used together with .list-inline-item on each <li> elements)	Try it
.pre-scrollable       |	Makes a <pre> element scrollable
