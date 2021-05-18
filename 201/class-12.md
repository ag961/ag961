# Chart.js, Canvas


source:

> https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/
> https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage
> https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage
> https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors
> https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text



  Chart.js is a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. 

  The chart is rendered using `<canvas>` element.

### Basic usage

`<canvas>`  has only two attributes, width and height, which are optional. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. It can be styled just like any normal image. 

Fallback content can be inserted inside the tags.

The <canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. 

The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The <canvas> element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. 

The script includes a function called draw(), which is executed once the page finishes loading; this is done by listening for the load event on the document.


### Drawing shapes with canvas

Drawing takes into account coordinate grid. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y).

### Applying styles and colors

fillStyle = color
Sets the style used when filling shapes.
strokeStyle = color
Sets the style for shapes' outlines.

### Drawing text
The canvas rendering context provides two methods to render text:

`fillText(text, x, y [, maxWidth])` - fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
`strokeText(text, x, y [, maxWidth])` - strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

-----

[**<== BACK**](201-toc.md)
