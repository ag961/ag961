# Forms and JS Events

Source:
> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley

## Chapter 7: “Forms” (p.144-175)

Forms allow collection of information from users. Inofrmation is sent from the borowser to the server using **mame/value** pair.

### Types of forms

* Adding text:
  
  * Input: `type = "text"`

  * Password input: `type = "password"`
  
  * Text area: `<textarea>`

  * Date: `type = "date"`

  * Search box: `type = "search"`

* Making choices

  * Radio buttons: `type = "radio"`

  * Ckeckboxes: `type = "checkbox"`

  * Drop-down boxes: `<select>`

* Submitting forms

  * submit button: `type = "submit"`

  * image button: `type = "image"`

  * `<button>` allows more control over button appearance

* Uploading files

`<form>` - element where form control lives.
`<action>` - attribute, value is the URL that receives info. 

`<fieldset>` - groups form controls
`<legend>` - contains caption for `<fieldset>`

`<placeholder>` - attribute that shows text until user clicks

**Method**: get vs post;


## Chapter 14: “Lists, Tables & Forms” (pp.330-357)

### Lists

`list-style-type` property allows to style the bullet ppoint.

`list-style-image` image acts as bulet point.

`list-style-position` bullet points appear `inside` or `outside`.

### Table

Table properties:

* width

* padding

* text-transform - converts to uppercase

* letter-spacing, font-size

* border-top, border-bottom

* text-align

* background-color

* :hover - highlights a table row when a user's mouse hover over it.

* border-spacing, border-collapse

### Forms

Form properties allow styling of forms

* font-size

* color

* background-color

* backgroun-image


-----

Source:
> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley

## Chapter 6: “Events” (pp.243-292)

### Event types

* UI Events
  * load
  * unload
  * error
  * resize
  * scroll

* Keyboard events
  * keydown
  * keyup
  * keypress

* Mouse events
  * click
  * dbclick
  * mousedown
  * mouseup
  * mousemove
  * mouseover
  * mouseout

* focus events
  * focus/focusiin
  * blur/focusout

* form events
  * input
  * change
  * submit
  * reset
  * cut
  * copy
  * paste
  * select

### Three ways to bind an event to an element:

1. DOM level 2 event listeners - **favored way**

2. Traditional DOM event handlers

3. HTML event handlers - **bad practice**


-----

[**<== BACK**](201-toc.md)
