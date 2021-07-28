# Docs for the HTML canvas Element & Chart.js

- [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Charts and Canvases

### Chart.js

When wanting to work with a pie, line, or bar chart. They are simular in a way, all start making a canvas. This canvas has our ID we grab and paste the DOM to, and we set our height and width. From there we have our data, in each type of chart, they have their own syntax for data, although, bar and line graph are simular. After we have our data, we then paste it to the DOM we made with our canvas element. Pasting to the DOM is the same for each, just depending on what your passing through. `new Chart(DOM variable).chartType(data);`

### Canvas Element

If you do not set a width or height, the default width is 300px, and 150px high. 

`canvas.getContext('2d');` is for rendering content and the canvas element understands that you want to render a 2d model.

### Checking for Support

Using fallback content in case some browsers do not fully support canvas will help it render even if it does not need it. For displaying our content with `canvas.getContext('2d');`, we can run an if statement that says `if (canvasVariable.getContext)` will support it with 2d, and if not, then you would write an else that then writges unsupported code for the browser.

This is a skeleton template

`<!DOCTYPE html>`
`<html>`
&nbsp;&nbsp;`<head>`
&nbsp;&nbsp;&nbsp;&nbsp;`<meta charset="utf-8"/>`
&nbsp;&nbsp;&nbsp;&nbsp;`<title>Canvas tutorial</title>`
&nbsp;&nbsp;&nbsp;&nbsp;`<script type="text/javascript">`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`function draw() {`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`var canvas = document.getElementById('tutorial');`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`if (canvas.getContext) {`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`var ctx = canvas.getContext('2d');`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`}`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`}`
&nbsp;&nbsp;&nbsp;&nbsp;`</script>`
&nbsp;&nbsp;&nbsp;&nbsp;`<style type="text/css">`
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`canvas { border: 1px solid black; }`
&nbsp;&nbsp;&nbsp;&nbsp;`</style>`
&nbsp;&nbsp;`</head>`
&nbsp;&nbsp;`<body onload="draw();">`
&nbsp;&nbsp;&nbsp;&nbsp;`<canvas id="tutorial" width="150" height="150"></canvas>`
&nbsp;&nbsp;`</body>`
`</html>`

Taken from [Basic usage of canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)

### Shapes

There are many tools we can also use, one is with recatangles, once we know `fillRect()`, `strokeRect()`, and `clearRect()`. We can make basic shapes and modify them.

WHen we want to draw shapes. We have to know our positions, how far we want to go, possible angle, and etc. Using `.lineto()`, `.moveTO()`, and `.fill()`. We can see that lineTo represents moving from origin, to that spot, and create a line, moveTO does the same, but it does not draw a line, and when we are making a shape, and we want to fill it, fill creates the last line back to the start and fills it in with color for us.

This can get more complicated with more difficult shapes, more specific and odd angles. This is where math will really be useful knowing your calculations and angles.

### Colors

With colors, we can use `.fillStyle = colorFormula;` here. With color formular, you can use math equations and a nested for loop to create slight variations of each color and much more. Being able to either fill, or use strokeStyle or color just the lines will be valuable where needed. You can also `.fillRect()` as well for rectangle shapes.

### Line

You can draw lines with the axis that is based on the pixels of the screen. Using that, you can even alter the size, distance, style, width, add a cap, and even connect it with other lines. Some reasons why this would be very useful to learn is that you can use it as a background for a page, as you can alter the gradient to make a sunset, or even the ocean colors.

Line styles and line width can create just a little more detail, and even finishing it off with a line cap, that will go outside your end of your line, it will not overwrite your exsisiting line.

### Draw

Using the draw method, we can create words, position them to where to want, create outlines of the words, or fill them with specific colors.

Using all of these specfic things, a canvas is just a white board that is waiting for us to decorate it with colors, words, and styles to please our audience.

## Resources

- [Chart JS](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)
- [Chart.js docs](http://www.chartjs.org/docs/)
- [Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
- [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
- [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
- [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
