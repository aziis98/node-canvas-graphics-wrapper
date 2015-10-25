# node-canvas-graphics-wrapper
A package that wraps an html canvas to Java Graphics object.

# How to use

Here there is an example that draws a red line, an empty black rectangle and a green-filled circle:

```
var Graphics = require('node-canvas-graphics-wrapper')

// var canvas = $('#mycanvas')[0]
var canvas = document.getElementById('mycanvas')
var g = Graphics.createFromCanvas(canvas)

g.setColor('#FF0000')
g.drawLine(100, 100, 200, 200)

g.setColor('#000000')
g.drawRect(100, 100, 50, 50)
g.setColor('#00FF00')
g.fillCircle(300, 300, 50)
```
