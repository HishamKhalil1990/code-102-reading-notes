# Chart.js, Canvas
## Chart.js
#### Charts are a type of data visualizing layout. Types of charts:
 1. **Line chart `new Chart(canvasIdVar).Line(dataObject);`**
 2. **Pie chart `new Chart(canvasIdVar).Pie(pieData, pieOptions);`**
 3. **Bar Chart `new Chart(canvasIdVar).Bar(barData);`**

## Canvas
#### canvas is an element used to show a graphical features that are built up using JavaScript like for charts. The `<canvas>` element doesn’t need a `src` and `alt` attributes but it defined by `height` and `width` . While media elements can have a fallback content, canvas doesn’t have one. It used as a drawing surface for rendering context and manipulating them by a method called `getContext()` . for drawing a graphical shape, a grid layout is supported by canvas using coordinate (x,y). To draw a rectangle:
  - **filled rectangle `fillRect(x, y, width, height)`**
  - **rectangular outline `strokeRect(x, y, width, height)`**
  - **Clear a specified rectangular area `clearRect(x, y, width, height)`**
#### It also used to draw:
  - **path**
  - **triangle**
  - **move the pen**
#### For styling the canvas drawings, there are some style attributes can be used:
1. **Coloring the shape as using `fillStyle = color`**
2. **Drawing a semi-transparent shapes using `globalAlpha = transparencyValue`**
3. **Change the line stile as using `lineWidth = value`**
4. **Create a pattern for images using `createPattern(image, type)`**
