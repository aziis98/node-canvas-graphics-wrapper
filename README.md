# node-canvas-graphics-wrapper
A package that wraps an html canvas to Java Graphics object.

# How to use

Here there is an example that draws a red line, an empty black rectangle and a green-filled circle:

```javascript
var Graphics = require('node-canvas-graphics-wrapper')

// var canvas = $('#mycanvas')[0]                 // getting the canvas with jquery
var canvas = document.getElementById('mycanvas')  // or with document.getElementById()

var viewport = { width: 1920, height: 1080 }
var g = Graphics.createFromCanvas(canvas, viewport)

g.setColor('#FF0000')
g.drawLine(100, 100, 200, 200)

g.setColor('#000000')
g.drawRect(100, 100, 50, 50)
g.setColor('#00FF00')
g.fillCircle(300, 300, 50)
```
