# Links & Layouts || JS Functions

---

#### Links

**Links** are used to take the user to another webpage. This is achieved by using an `href` attribute through the `<a>` tag. Here are several different ways to achieve this:

* `<a href="mailto:john@example.com">Email John</a>` This will open the user's default emailing application with the selected link's email address as the recipient.
* `<a href="http://www.imdb.com" target="_blankj"> List of movies</a>` This will take the user to a new link in a **new tab.**
* `<a href="#top"> Top of page</a>` This will take the user to the  html element with **id of top.**
  
---

#### Layouts

In CSS, it is important to understand how the elements are placed in relation to each other. There are three primary ways in which elements can *flow*.



**Normal Flow**
All block level elements are on a new line. This is the default html positioning. `position: static`

**Relative Positioning**
Moves elements from normal flow to a different position with it's 'box'. `position: relative;`

**Absolute Positioning**
Moves element out of normal flow and other elements act as if it is not even present. The element can be moved in relation to it's containing element. This element will move when the user scrolls up or down. `position: absolute;`

**Fixed Positioning** is another type of absolute position. Instead of the element moving in relation to it's containing element, it moves in relation to the browser window. The element does not move when the user scrolls up or down. `position: fixed;`

**Z-index**
When using relative, absolute or fixed positioning, it is important to note that those elements are taken out of normal flow, so it is possible for elements to overlap or stack on top of each other. The html tags that are further down the script will appear on top by default. But it is possible to control which element will appear on top by using a z-index. A z-index with a greater value will appear on top.

`z-index: 10;`

**Floats**
Floating elements to the left or right will allow other elements to *flow* to the left or to the right of it. This can cause issues with some succeeding elements. To fix issues you may be having with elements sitting in the wrong position, the **clear** property will prohibit any elements from touching the given side of the element.

```css
float: left;
float: right;
clear: left;
clear: right;
clear: both;
```

**Fixed layout vs Liquid layout**
A fixed layout will not adjust according to the user's screen size. Typically, a fixed layout has measurements of pixels. This can be easy on the user for designing the website, but it will also not adjust the content size based on what device the client is using.

A liquid layout is built using percentage values. This will allows the content to adjust when the browser is resized or if the user has a different screen size than the developer.

---

#### JavaScript Functions

##### What is a Function?

A function is a way to group together code that will complete a specific tasks.
Benefits of using functions:

* Code Reusability
* No repetitive code
* Better script organization

Example:

```javascript
function greet() {
  console.log('Hello!');
}
```

---

#### Pair Programming

Pair programming refers to having two people working on a project. One of the individuals is the **driver** and the other is the **navigator**. The driver is the one to actually type out the scripts while the navigator handles file management, the text editor and version control. The navigator is also responsible for scanning for bugs and algorithm solutions.

Benefits of pair programming:

* Collaboration
* Learning from others
* Career readiness
* Enhance teamwork capabilities
