# HTML/CSS - lists & Boxes | JavaScript - Decisions & Loops

---

#### Lists 

When using HTML, keep in mind that there are three different **lists** we can use to give our site more structure.
  
* **Ordered Lists**
* **Unordered Lists**
* **Definition Lists**

**Ordered lists** utilize numbers to order each list item. The element `<ol>` signifies that an ordered list is being used. These lists can be beneficial for when ordering something that needs to be done as a sequence, such as a recipe or a manual of some sort.

`1. Step one.`
`2. Step 2.`
`3. Step 3.`
`4. Step 4.`
`5. Step 5.`

**Unordered lists** use the asterisk `*` to mark each list item. When using an unordered list, use the `<ul>` tag.

`Breakfast food`

* `Eggs`
* `Orange Juice`
* `Bacon`
* `Hash Browns`

Ordered and unordered lists require child `<li>` tags to signify each list item.

---

#### Boxes

CSS treats all html elements as boxes. This allows CSS rules to manipulate the dimensions of the targeted box in various ways. Width and height can be adjusted by:

`width: 250px;`
`height: 25%;`

 The width and height can also be limited to a certain size so that when the browser is resized smaller (or larger).

 `min-width: 50px;`
 `min-height: 75px;`
 `max-width: 80%;`
 `max-height: 75%;`

 The **Margin** property provides space between the targeted box and any surrounding elements, while the **padding** property increases space from the box to the content held within the same box. 

 `margin: 20px;` 20px space on all sides
 `margin: 20px 10px;` 20px space on top and bottom, 10 px space on left and right
 `margin: 20px 10px 5px;` 20px space on top and bottom, 10px space on right, 5px space on left
 `margin: 5px 10px 15px 20px;` 5px space on top, 10px right, 15px bottom, 20px left

 If it isn't clear, the space applied to the margin is done in a clockwise manager starting from the top border. The first three statements show a shorter hand version to apply spacing. Applying padding space is done in the same manner.

 ---

#### Decisions & Loops

**Switch Statements** are similar to if statements, but instead of checking a condition, it compares a variable to a series of 'cases'. If a case matches the value of the variable, that specific case is executed. Each case should end with a `break;` statement in order to break out of the switch statement when a match is found. 

JavaScript is a **weakly typed** language because it does not require data type specificity when creating variables. When comparing two values it only checks the values of the variables instead of the data types, UNLESS the strict `===` equality is being used. This is why is it best practice to use strict equality in JavaScript.

**Short Circuit Values** occur when a logical operator does not need to check the second expression. The following is a short circuit value because the OR operator only needs one of the two expressions for the overall expression to equate to true. Since the first expression is true, there is no need to continue to evaluate the second expression.

`(5 < 6) || (4 > 3)`

**Loops** are used to iterate through a specific statement a certain number of times. There are three main types of loops:

1. for loops
2. while loops
3. do while loops

A **for loop** should be used if the amount of loop iterations can be anticipated.

```javascript
for(var i = 0; i < 10; i++) {
  `console.log(i);
}
```

A **while loop** should be used if the amount of loop iterations can NOT be anticipated.

```javascript
var i = 0;
while (i < 10) {
  console.log(i);
  i++;
}
```

A **do while loop** is very similar to the while loop but that the condition is checked AFTER the code is ran. This will cause the loop to run at least once even if the condition is false.

```javascript
var i = 0;
do {
  console.log(i);
  i++;
} while (i < 10)
```
