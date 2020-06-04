# Regular Expressions & Regex101 || Grid

---

### Regular Expressions

**Regular Expressions** are used to find or match specified characters to a string. They can also be used to replace those specified characters.

The **match** method returns the matched characters.

```js
let string = 'hello world!';
let regex = /lo/;
string.match(regex);
```

The **test** method returns true or false if the specified characters are found or not.

```js
let string = 'hello world!';
let regex = /lo/;
test(string);
```

**Regex101** is a user friendly guide that helps create regular expressions.

[Regex101 website](https://regex101.com/)

---

### Grid

The CSS **grid** layout tools are a streamlined and efficient to design the layout of a website. It controls both **columns** and **rows**. This means that it is a **2D** layout, where flexbox is a single dimension layout.

Defining a grid: 

```css
main {
  display: grid || inline-grid;
}
```

For a detailed description of the properties and values that grid offers, click [here](https://css-tricks.com/snippets/css/complete-guide-grid/).