# Introductory HTML and JavaScript

As summurized from 

> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley  

## HTML Chapter 1: “Structure” (pp.12-39)

In HTML we use ***tags*** to make the web page look exactly how we want it. The tag consists of a code placed betweer `<` and `>` (angled brackets). An item wrapped between two tags (opening and closing), is an ***element***.  

Examples:

`<p>` - paragraph

`<body>` - what to show inside the main browser window

`<head>` - information about the page

`<title>` - text shown in the top of browser or on the tab

The opening tag of an element can also have ***attributes*** made up of a ***name*** and a ***value***.

* `<p lang="en-us">Paragraph in English</p>`
  * *lang* is name, *en-us* is value.

## HTML Chapter 8: “Extra Markup” (p.176-199)

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


## HTML Chapter 17: “HTML5 Layout” (pp.428-451)

HTML5 is a version of HTML that has a new set of elements that allows you to divide up the parts of a page (previously `<div>` elements).

Examples are:
`<header>, <nav>, <article>, <footer>, <section>, <aside>, <hgroup>,  <figure> and <figcaption>`.

`<a>` - allows to turn an entire block into a link.

## HTML Chapter 18: “Process & Design” (pp.452-475)  

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

-----

As summarized from

> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley  

## Introduction  

JavaScript is a language that gives developers lots of abilities to program their web-sites to interact with users. It can access contents of a page, modify it, and react to scpecific events happening on the page.  

## JS Chapter 1: “The ABC of Programming” (pp.11-52)  

JavaScript works by means of **scripts**, which are instructions that a computer can follow. A computer is very obedient, and will do exactly what we tell it to do. But instructions have to be very specific, step-by-step. And unlike humans, computers don't learn, so they have to be told what to do everytime they run a script.

Scripts have to be carefully designed. A big first step is creating a ***flowchart***, which is a diagram that resembles a protocol. It gives everyone a picture of how things should run ste-by-step.

JavaScript is a separate layer that builds on HTML and CSS. Using JS, we can change how the pages behaves, adding interactivity.  

It's best to keep JS code in its own file with ".js" extension.

`<script>` element is used in HTML to link the browser to JS file.

-----
[**<== BACK**](201-toc.md)
