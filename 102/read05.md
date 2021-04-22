# Design web pages with CSS  

> As summurized from Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley  

**CSS** stands for ***C***ascading ***S***tyle ***S***heets. While HTML holds our web-site's content, CSS in turn allows us to manage visual appearance of such content. Using CSS we can choose fonts and colors for our text, its size, add background colors to the page and to each box. CSS comes in especially handy when we have to manage several pages. It gives us ability to create ***rules*** that specify how each element within HTML code will appear. All we have to do is change one rule specific to the element. And if that element is present on differnet pages, the rule will equally apply to all of those elements at the same time, no matter where they are. Thus, controlling appearance of web pages becomes a lot more easy and less time consuming.  

### Chapter 10: Introducing CSS

CSS rule contains a ***selector***  and a ***declaration***. A declaration has a ***property*** and a ***value*** separated by colon.

```
p {
  font-family: Arial;}
```
ALthough CSS rules can be written within HTML, it is better to create an external CSS and refer to it from within HTML by using:

`<link href="css/styles.css" type="text/css" rel="text/css">`

It lives inside `head` element, and attribute `href` specifies path to CSS file.

#### CSS cascade:

* **Last rule** - latter of two identical selectors take precedence
* **Specificity** - more specific rule takes precedence
* **Improtant** - add `!improtant` to property value to increase it precedence.

### Chapter 11: Color

`color` property specifies color of the text inside an element in one of three ways:

* RGB values
* HEX codes
* Color names

`background-color` property gives color to a box of an element. If no color specified, the background is transparent.

* `opacity` can be added to specify opacity level. Value is between 0.0 and 1.0.  

* `hsl (0,0%,50%)` - Hue (0-360), Saturation, Lightness.  
  * `hsla` - HLA + transparency (0-1.0)

-----

[**<== BACK**](102-toc.md)