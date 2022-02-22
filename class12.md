# Class 12 – Docs for the HTML <canvas> Element & Chart.js
  
## Reading Notes Overview 12
  
### HTML book
  
#### Charts.js API Article
  
- Charts are better at displaying data than tables.
- They are visually appealing and convey data quicker.
- Chart.js is a JavaScript plug-in that uses HTML5’s canvas element to draw graphs on the webpage.
- Chart.js allows you to create bar charts, line charts, pie charts, etc.

#### Canvas API Basic Usage
  
- The <canvas> element resembles the <img> element, and the only clear difference is the <canvas> element doesn’t have the “src” or “alt” attributes.
- The <canvas> element only has the “width” and “height” attributes, which are optional and can also be set up using DOM properties.
- The default <canvas> settings for width and height are 300 pixels wide and 150 pixels high.
- You can use CS to size the <canvas> element.
- It’s a good idea to apply an “id” attribute to the <canvas> element so it’s easier to identify in the script.
- Providing fallback content with the <canvas> element makes it easier for older browsers to display content. 
- If a browser doesn’t support <canvas>, then it will ignore the content inside the container and render the content normally.

#### Drawing shapes with canvas
  
- The <canvas> element is drawn in a grid, or coordinate space.
- One unit in the grid corresponds to one pixel on the canvas.
- The grid is positioned on the (0,0) x-y axis as the origin. All elements are placed relative to the origin.
- The <canvas> element only supports primitive shapes, such as rectangles and lists of points connected by lines (i.e., paths).
- In order to create other shapes, you’ll need to combine one or more paths.

#### Applying styles and colors
  
- You can also apply colors, transparency, line styles, gradients, patterns, and shadows.
- Use CSS <color> values when adding color, as color is a string representative in CSS.
- There are canvas fill rules for determining if a point is inside or outside a path, thus if the point gests filled in or not.
- The rules that make up this rule are non-zero and even-odd winding rules.
- Then nonzero rule is used to determine if a point falls inside an enclosed curve.
- The even-odd rule is used to determine how a shape with more than one closed outline is filled.
  
#### Drawing text
  
- You can render text in two ways: 1. Fill in the text an x-y position, or 2. Strokes at an x-y position.
- Font can be used to style text. Such as the font property, text-align, textBaseline, and direction
