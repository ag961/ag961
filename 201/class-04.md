# HTML Links, CSS Layout, JS Function

As summarized from:

> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley

and

> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley

## Chapter 4: Ch.4 “Links” (pp.74-93)

`<a href="http://google.com">Google</a>` - link format.

**Relative URL** - If linking to pages within the same site, no need to specify domain name.

`mailto:` - email links.

`target="_blank"` - opening a new window

Use *id* attribute to link to a specific part of the page and `#` to call.


## Chapter 15: “Layout” (pp.358-404)

Every HTML element is a box, either a block level or an inline box.

**Containing (parent) element** - a block-level element that houses another block level element (**child**). 

*Position* property:

* static

* relative (in relation to where it would have been in normal flow).

* absolute - doesn't affect position of other elements.

* fixed - in relation to browser window.

*Z-index* - controls which element sits on top if there is an overlap. Higher number sits on top.

*Float* - elements become block-level, around which other content can flow (to right or left of it). Also used to place elements side by side.

### Layouts

* Fixed width - do not change size when browser window size changed.

* Liquid - stretch and contract in realtion to browser window size.

* Grids - help structure the page. 


## Chapter 3 : “Functions, Methods, and Objects” (pp.86-99)

### Functions and Methods

Functions let you group a series of statements to perform a specific task and avoid repeating the same code. When you ask the function to perform its task, it is known as ***calling*** the function. The response of a function is known as a return value. Functions can be reused.

To declare a function we use `Function` keyword. Is it followed by fucntion name and `()`, then `{ code block }`.
Sometimes a function needs spesific information (parameters to work). Arguments are actual values passed into the code.

``` markdown
function getArea (width, height) {
  return width * height;
} 
```

Variable scope - wheere the variable can be used (inside vs outside of fucntion). Global variables use more memory vs local variables.

## Article: “6 Reasons for Pair Programming”

> Grampa, A (2018). *6 Reasons for Pair Programming*. Retrieved from: https://www.codefellows.org/blog/6-reasons-for-pair-programming/ 

**Pair programmimg** - using two people to work on a coding task: a driver and navigator. Driver does the typing, navigator - guides the driver, thinks about a bigger picture, checks for typos. 

6 reasons to use it:

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environments readiness


-----
[**<== BACK**](201-toc.md)