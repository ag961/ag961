# Structure web pages with HTML

> As summurized from Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley

***HTML*** stands for Hyper Text Markup Language. It is one of the languages that authors use to create and style their web pages. 

## Process & Design (Chapter 18)

The process of building a web pages is similar to starting your own business. Just like having to make a business plan first, the approach to making a web page has to be carefully thought-out.

### Identify the following:

* Target Audience - **Who** will be interested in visiting

* Motivation and goals - **Why** are they coming to your page.

* Key information - **What** information do they need to achieve their goals

* Frequency of updates - depends on **how often** people will visit/return

### Orginizing information

* **Site map** - basic diagram that helps you identify and group information that will go to each page.

* **Wireframes** - visual placement of information (items, boxes of text, images, etc.) on each page. Helps you allocate space.

### Visual Design

Author employs **visual hierarchy** to organize and prioritize the content in a way that makes it easy for a visitor's eye to perceive information. Here we focus on size, color, style, contrast, spacing and use of images.

## Structure (Chapter 1)

In HTML we use ***tags*** to make the web page look exactly how we want it. The tag consists of a code placed betweer `<` and `>` (angled brackets). An item wrapped between two tags (opening and closing), is an ***element***.  

Examples:

`<p>` - paragraph

`<body>` - what to show inside the main browser window

`<head>` - information about the page

`<title>` - text shown in the top of browser or on the tab

The opening tag of an element can also have ***attributes*** made up of a ***name*** and a ***value***.

* `<p lang="en-us">Paragraph in English</p>`
  * *lang* is name, *en-us* is value.

## HTML5 Layout (Chapter 17)

HTML5 is a version of HTML that has a new set of elements that allows you to divide up the parts of a page (previously `<div>` elements).

Examples are:
`<header>, <nav>, <article>, <footer>, <section>, <aside>, <hgroup>,  <figure> and <figcaption>`.

`<a>` - allows to turn an entire block into a link.

## Extra Markup (Chapter 8)  

`<!DOCTYPE html>` - specisies version of HTML. Should be first thing in a document.

`<!-- text -->` - comment not visible to a user

ID attribute `<(tag) id="...">` - uniquely identifues element

CLASS attribute `<(tag) class="...">` - unique group of elements

`<div>` - group a set of elements in one block-level box

`<span>` - inline grouping

`<iframe>` - inline frame (often to insert a Google map). Used with attributes `src`, `height`, `width`, `scrolling`, `frameborder`, `seamless`.

``` markdown
<meta (attribute)="value"
  conent="value" />
```

- empty element, contains info about web page for search engines, not visible to users.  

`<&>` - escape character

-----

[<== BACK](102-toc.md)
