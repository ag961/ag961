# Class 6: Problem Domain, Objects, and the DOM

## Problem Domain

source:
> Sonmez, J. (2015). *Understanding The Problem Domain Is The Hardest Part Of Programming.* Retrieved from: https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming

Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.
The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.

Having a clear picture of what the code should do, and why exactly that way, is the most critical piece. 

To make programming easier, we can do one of two things:

1. Make the problem domain easier:  take a part of the problem and fully understand that part before expanding the problem domain
2. Get better at understanding the problem domain: make sure you understand a problem inside and out before you try and solve it with code



-----

from:
> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley

## Chapter 3: “Object Literals” (pp.100-105)

Objects group together a set of variables and functions to create a model of something you would recognize from a real world. In an object, variables become known as properties and functions become known as methods.

**Key** is a name of a property or a method in an object. No two same-named keys in an object. Value of a property can be a string, number, Boolean, array, or another object. Value of a method is always a function.

Each key is separated from a value by a colon. Each property and method with a comma.

Access the property or a method using dot notation.

## Chapter 5: “Document Object Model” (pp.183-242)

The DOM tree is a model of a page, stored in a browser's memory. Every element, attribute, and a piece fo text in the HTML is represented by its own DOM node. Scripts access and update this DOM tree (not the source HTML).

Attribute nodes are not children of the elements, but a part of that element. Text nodes cannot have choldren.

Accessing and updating the DOM tree involves two steps:

1. **Locate the node**
2. **USe its text content, child elements, andd attributes**

**Selecting an individual element**:

* getElementBy ID()
* querySelector()

**Selecting multiple elements**:

* getElementByClassName()

* getElementsByTagName()

* querySelectorAll ()

**Traversing between element nodes**:

* parentNode

* previousSibling/nextSibling

* firstChild/lastChild

**Access/update text nodes**

* nodeValue

**Work with HTML content**

* innerHTML

* textContent

* createELement()

* createTExtNode()

* appendChild()/removeChild()

**Access or update attribute values

* className/id

* hasAttribute()

* getAttribute()

* setAttribute()

* removeAttribute()

-----

[**<== BACK**](201-toc.md)