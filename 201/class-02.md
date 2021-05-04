# Basics of HTML, CSS & JS

-----

As summarized from 
> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley  

## Chapter 2: “Text” (pp.40-61)

### Structural markup

* Headings: HTML has 6 level of headings `<h1>` thourgh `<h6>`.
* Paragraphs: `<p>...</p>`
* Bold and Italic: `<b>` and `<i>`
* Superscript: `<sup>`; Subscript: `<sub>`
* Line break: `<br />` (empty element)
* Horizontal rule: `<hr />` (empty element)

### Semantic markup

* `<strong>` - to indicate content with strong importance (turns text bold by default)
* `<em>` - emphasis that subtly changs the meaning of a text (italics by default)
* Quotations
  * `<blockquote>` - paragraph long quotes
  * `<q>` - shorter quotes within paragraph
* `<abbr title="...">abbreviation</abbr>` - abbreviation or acronym
* `<cite>` - citation; `<def>` - definition


## Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

**CSS** stands for (***C***)ascading (***S***)tyle (***S***)heets. While HTML holds our web-site's content, CSS in turn allows us to manage visual appearance of such content. Using CSS we can choose fonts and colors for our text, its size, add background colors to the page and to each box. CSS comes in especially handy when we have to manage several pages. It gives us ability to create ***rules*** that specify how each element within HTML code will appear. All we have to do is change one rule specific to the element. And if that element is present on differnet pages, the rule will equally apply to all of those elements at the same time, no matter where they are. Thus, controlling appearance of web pages becomes a lot more easy and less time consuming.  

CSS rule contains a ***selector***  and a ***declaration***. A declaration has a ***property*** and a ***value*** separated by colon.

```
p {
  font-family: Arial;}
```
ALthough CSS rules can be written within HTML, it is better to create an external CSS and refer to it from within HTML by using:

`<link href="css/styles.css" type="text/css" rel="text/css">`

It lives inside `head` element, and attribute `href` specifies path to CSS file.

### CSS cascade:

* **Last rule** - latter of two identical selectors take precedence
* **Specificity** - more specific rule takes precedence
* **Improtant** - add `!improtant` to property value to increase it precedence.

-----
As summarized from

> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley  

## Chapter 2: “Basic JavaScript Instructions” (pp.53-84)

A script is a series of instructions (known as ***statements***), that a computer can follow one-by-one.

Comments explain what your code does Multi-line comments are between `/*` and `*/` caracters. Single-line comments follow two slashes `//`

***Variables*** is where a script temporarily stores information.

### Steps:

1. **Declare the variable** - create and give it a name

2. **Assign a value to the variable** - what information to store

### Rules to follow in giving variable a name:

1. The name can only begin with a letter, "$", or "_".
2. Nmame can contain letters, numbers, "$". or "_". No "-" or ".".
3. No keywords or reserved words.
4. Variables are cas sensitive.
5. Name should describe what variable stores.
6. More that 1 word - second word starts with Uppercase or "_"

## Chapter 4: “Decisions and Loops” (pp.145-162)

### Comparison Operators

* `==` - equal to
* `===` strict equal to (both data type and value are the same)
* `!=` - is not equal to
* `!=` - strict not equal to
* `>` - greater than
* `>=` - greater than or equal to
* `<` - less than
* `<=` - less than or equal to

### Logical Operators

* `&&` - Logical AND. If both expressions are true, then true. Otherwise returns false
* `||` - Logical OR. If either is true, then returns true. If both false, returns false.
* `!` - Logical NOT. Takes a single Boolean value and inverts it.

### Loops

**For** loop. Runs a code a specific number of times.  

`for (var i = 0; i < value; i++) { code to execute during loop}`

Where `var i = 0;` is initialization. `i<10;` is condition. `i++` is update

**While** loop.  Condition can be other than the counter, and the code will continue to loop as long as the condition is true.

### If ... Else

The if...else statement checks a condition. If it resolves to true the first code block is exectued. If it resolves to false the second code block is run.

```
if (a > b) {
  function1();
}
else {
  function2();
}
```

-----

[**<== BACK**](201-toc.md)