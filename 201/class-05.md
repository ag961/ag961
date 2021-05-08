# HTML Images, CSS Color and Text

Source:  
> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley


### Chapter 5: “Images” (pp.94-125)

* `<img>` - adds an image.

***Following are attributes***:

* `source` - location of the image;
  
* `alt` - text description;

* `title` - additional info about the image;

* `height` - height

* `width` - width

Height and weight is preferably done in CSS.

`<img>` is an inline element. To make it into a block-element in CSS  `display: block`.

`float` property is used to push an image to right or left so other elements can surround it.

Size can be specified in pixels, ems, vw, %, etc.

### Chapter 11: Color (pp.246-263)

`color` property specifies color of the text inside an element in one of three ways:

* RGB values
* HEX codes
* Color names

`background-color` property gives color to a box of an element. If no color specified, the background is transparent.

* `opacity` can be added to specify opacity level. Value is between 0.0 and 1.0.  

* `hsl (0,0%,50%)` - Hue (0-360), Saturation, Lightness.  
  * `hsla` - HLA + transparency (0-1.0)

### Chapter 12: “Text” (pp.264-299)

`font-family` porperty aloows you to speify the typeface.
`font-size` can be specified in pixels, percentages, ems, pt.
`font-weight: bold` - makes text bold.
`font-style:` `italic`, `oblique`.
`text-transform` - `uppercase`, `lowercase`, `capitalize`.
`text-decoration` - `underline`, `overline`, `none` (removes decorations for links).

Spacing:
`line-sapcing` - between lines;
`letter-spacing` - between letters;
`line-height` - space above line.
`text-alignment` - left, right, center, justify (takes up full length.)
`text-indent` - indents first line of text.

-----

[**<== BACK**](102-toc.md)