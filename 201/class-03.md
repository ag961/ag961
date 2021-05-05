# HTML Lists, Control Flow with JS, and the CSS Box Model

As summarized from:

> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley  

## Chapter 3: “Lists” (pp.62-73)

`<ol>` - Starts ordered lists (numbered).

`<ul>` - Starts unordered lists (bullet points).

`<li>` - Each item in the list is placed between those.

`<dl>` - definition list; consists of series of terms (`<dt>`) and their definitions (`<dd>`).

**Nested lists** are created by starting a second list inside of `<li>` element.

In CSS use **list-style-type** property to spcify the look of list elements.

## Chapter 13: “Boxes” (pp.300-329)

`height` and `width` properties control the size of boxes.

**Pixels** (`px`) - accurately controls the size in pixels

**Percentages** (`%`) - box is relative to the size of the browser window or to the size of containing box.

**Ems** (`em`) - size of the box is based on the size of text within it.

*Min-width*, *min-height* - smallest size a box can be
*Max-width*, *max-height* - maxi width a box can be

*Overflow* property:
* `hidden` - hides extra content that doesn't fit in box
* `scroll` - adds scrollbar

Border properties:
* `margin` - space outside the edge of border. To center the box, set *left-margin* and *right-margin* to auto 
* `padding` - space between border and inside content
* `border-width` - size of border line
* `border-style` - solid, dotted, etc.
* `border-color` - color
* `border` - shorthand to specify width, style and color in that order.
* `border radius` - to round the corners
* `box shadow` - adds drop shadow around the box
* `border image` - applies image to the border

`display` property allows to turn inline element into a block level.

-----
As summarized from:

> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley

## Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)

**Array** is a special type of variable that stores a list of values. The values then can be accessed as if they are a numbered list (starts at zero).

Example: 

```
let colors;
colors = ['white', 'black', 'custom'];

let itemThree;
tiemThree = colors[2];
```
Values can also be changed later:
``` 
colors[2] = `beige`
```

## Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)

### Switch statement format

```
switch (level) {
  case 'One':
    title = 'Level 1'
    break;
  
  case 'Two`:
    title = 'Level 2';
    break;
    
  case 'Three':
    title = 'Level 3':
    break;

  default:
    title = 'Test';
    break;
}
```
When the match is found, that code is run, then break command makes switch statement to stops reading further.

### Coersion and weak typing

JavaScript can convert data type (weak typing). This is known as type coercion.

**Falsy** values are treated as if they are false.
**Truthy** values are treated as if they are true.

### Loops

**For** loop. Runs a code a specific number of times.  

`for (var i = 0; i < value; i++) { code to execute during loop}`

Where `var i = 0;` is initialization. `i<10;` is condition. `i++` is update

**While** loop.  Condition can be other than the counter, and the code will continue to loop as long as the condition is true.

Format: 

```
let i = 1;
let msg = ` `;

while (i < 10) {
  msg += i + ` x 5 = ` = (i * 5) + `<br />`;
  i++
}
```

-----
[**<== BACK**](201-toc.md)
