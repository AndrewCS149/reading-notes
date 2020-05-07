#CSS Layout

---

#### Positioning Concepts

Different html elements render differently according to their tag name.

- block level elements - each start on a new line
- inline elements - flows between elements as long as it is narrow enough

A **containing** element refers to the outer most block level element of nested block level elements. For example; the `<div>` tag is often used as a containing as it will group many other elements inside of its tags. Grouping together elements can help in structuring a web page.

---

#### Positioning Schemes

Three main positioning schemes 

```css
position: normal;
position: relative;
position: absolute;
```

The `z-index:` property can control which element appears on top (or bottom) of overlapping elements. An element with a higher z-index value will appear on top of those with lower values.

---

#### Different Screen Sizes

There are many different screen sizes out there which makes it important to have a dynamic page that will adapt to each size. This is known as a **liquid** layout.

A liquid layout can be achieved by using sizing values of percentages, viewport width `vw;` and viewport height `vh;`.

