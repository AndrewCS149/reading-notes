# CSS: Transforms || Transitions || Animations

---

#### Transforms

What are transforms?
Transforms have properties which can change elements.


Syntax: 

```css
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```

The transform property has two settings, **2d** and **3d**.

2D transforms work on an **x and y axis**.
**Translate** will push an item around instead of resizing it.
 Examples:
 
```css
.div {
  transform: scale(1.50);
  transform: scaleX(1.25);
  transform: scaleY(.75);
  transform: rotate(70deg);
  transform: translate(-10px, -15px)
  transform: translateX(10px)
  transform: rotate(50deg) scale(1.25);
}
```

3D transforms expand not only on an x and y axis, but also on the **z axis**.

```css
.div {
  transform: perspective(150px) rotateZ(45deg);
}
```

---

#### Transitions and Animations

A **transition** occurs when the state of an element changes interactively. This can be used with properties like `:active` and `:hover`.

**Animations** are like transitions but the end state of an object's appearance occurs in multiple frames allowing the user to see the changes taking form.

Transition example:

```css
.div {
  background-color: blue;
  transition-property: background;
  transition-duration: 2s;
  transition-timing-function: linear;
}

.div:hover {
  background: red;
}
```
