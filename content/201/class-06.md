# DOM and Object Literals

---

#### The Problem Domain

Understanding the **problem domain** is one of the most crucial parts in programming. Outlining exactly what issues will be faced makes programming much more simple. This can be achieved by:

- Identifying use cases
- Examine each identified 'problems' in pieces

---

#### Object Literals

**What is an object?**

An object is a set of variables, methods and function that are placed together to form an **object**. An object has properties, much like a car has four wheels, a color, and requires a specific type of fuel.

```javascript
var car = {
  make: 'bmw',
  model: '328i',
  color: 'silver',
  fuelType: '87 gas'
};
```

---

#### DOM (Document Object Model)

The **DOM** essentially tells the browser how the html should be displayed in a web browser and how the JavaScript interacts and creates changes while inside of that browser. The term **API** (Application Programming Interface) and DOM are used interchangeably.

The **UI** (User Interface) is the elements that create how the user sees and interacts with an application.

There are methods that are used to retrieve different elements or **nodes** and change them directly. These are referred to as **DOM queries**.

`document.getElementById('name');`

| Object     | Method                   |
| ---------- | ------------------------ |
| `document` | `getElementById('name')` |

| DOM query                         | Method                    |
| --------------------------------- | ------------------------- |
| `document.getElementById('name')` | `getAttribute('class')';` |

Navigating through the DOM can allow software developers to access any HTML element. Those elements can then be updated or deleted.
