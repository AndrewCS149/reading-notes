# Chart.js || Canvas Tag || Shapes || Text

---

#### Chart.js

**Chart.js** is a library that is full of existing bar charts. This makes bar charts easy to use.

To download, go to the chart.js repo and clone the repo to a local machine. Then attach the library by using a script tag.

```js
<script src="chart.min.js"></script>
```

Now all of the functionality can be used from chart.js.

Line chart:

```js
<canvas id="buyers" width="600" height="400"></canvas>
```

```js
<script>
  var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);

  var buyerData = {
    labels : ["January","February","March","April","May","June"],
    datasets : [
      {
        fillColor : "rgba(172,194,132,0.4)",
        strokeColor : "#ACC26D",
        pointColor : "#fff",
        pointStrokeColor : "#9DB86D",
        data : [203,156,99,251,305,247]
      }
    ]
  }
</script>
```

Example above taken from "https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/".

---

#### Canvas Tag

The canvas has two attributes, **width** and **height**, which are both optional attributes.

The canvas element is used to draw on. This is how the bar charts will be applied to an html page.

---

#### Shapes

Shapes can be drawn to the grid that is provided with the canvas element.

- Rectangles
- triangles
- lines
- Arcs
- Quadratic Bezier curves
- Cubic Bezier curves


Shape methods:

```js
fillRect(x, y, width, height);
strokeRect(x, y, width, height);
clearRect(x, y, width, height);
```

The above syntax can be applied to most shapes.

Styling can also apply to these shapes. 

```js
fillStyle = 'blue';
strokeStyle = 'green';
```

Line Styling:

```js
lineWith = value
lineCap = type
lineJoin = type
miterLimit = value
getLineDash()
setLineDash(segments)
lineDashOffset = value
```

Gradients:

`createLinearGradient(0,0, 200, 200);`

---

#### Text

Rendering text:

```js
fillText(text, x, y [, maxWidth])
```

or

```js
strokeText(text, x, y [, maxWidth])
```

example:

```js
fillText('hello world', 10, 50)
strokeText('hello world', 10, 50)
```
