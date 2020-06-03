# Mustache.js || Flexbox 

---

# Mustache.js

#### JavaScript Templating

A quick and simple way to render client-side templates.

#### Mustache Templating

```js
Mustache.render("hello, {{name}}", {name: "Andrew"});
// returns: Hello, Andrew
```

---

# Flexbox

**Flexbox Layout**: A better, simpler way to layout and align a page.

This is a good approach for aligning elements when there dimensions are unknown.

Defining a flex container: 

```css
.div {
  display: flex;
}
```

Flex wrap - Tries to fit all elements on one line.
```css
.div {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

