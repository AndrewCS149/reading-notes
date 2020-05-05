# HTML Tables || JS Function, Methods and Objects

---

#### Tables

The `<table>` element is used to create different tables of related data. Example could be the rankings of a sports team or different country populations. 

Much like the an unordered list, the table element requires different child elements.

```html
<table>
  <tr>

    <tr>
      <th>Sunday</th>
      <th>Monday</th>
      <ht>Tuesday</th>
    </tr>

    <td>1pm</td>
    <td>Meeting 1</td>
    <td>Meeting 2</td>
    <td>Meeting 3</td>
  </tr>

  <tr>
    <td>2pm</td>
    <td>Meeting 1</td>
    <td>Meeting 2</td>
    <td>Meeting 3</td>
  </tr>
</table>
```

will display as:

 |      | Sunday    | Monday    | Tuesday   |
 | ---- | --------- | --------- | --------- |
 | 1 pm | Meeting 1 | Meeting 2 | Meeting 3 |
 | 2 pm | Meeting 1 | Meeting 2 | Meeting 3 |


`<tr>` stands for **table row** and `<td>` stands for **table data**.

---

#### Functions, Methods & Objects 

After creating a new object, an **instance** of that object needs to be created in order to actually use the object. This is accomplished by the **new** keyword.

```javascript
function car(make, model, currentSpeed) {
  this.make = make;
  this.model = model;
  this.topSpeed = currentSpeed;

  this.changeSpeed = function(speed) {
    return currentSpeed + speed;
  }
}
```

Now a new object needs to be **constructed** with the **new** keyword.

```javascript
var car1 = new car('bmw', '328i', 60);
var car2 = new car('ram', 'rebel', 45);
```

The `changeSpeed()` method can be invoked through these new instances:

```javascript
car1.changeSpeed(-10);
car2.changespeed(20);
```

Now car1 has a current speed of 50 while car 2 has a new current speed of 65.

---

#### Global JS objects

- Global JS objects normally start with a capital letter.
- The following are all examples of global objects:
  - String
  - Number
  - Boolean
  - Date
  - Math
  - Regex
