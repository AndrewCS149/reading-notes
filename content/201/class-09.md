# Forms, Lists and Tables || Javascript events

#### Forms 

HTML 5 uses forms as a way to retrieve client information. There are many variations of forms:

- adding text
  - Text input
  - Password input
  - Text area
- Decision making
  - Radio buttons
  - Checkboxes
  - Drop-down boxes
- Submitting forms
  - Submit buttons
  - Image buttons
  - file uploads

How do they work?

1. User fills out form and presses button
2. The form name and the information submitted is sent to the server
3. The server processes this information through another programming language
4. An appropriate action is sent back to the user

Form example: 

```html
<form action="http://www.example.com/" method="get">
  <p>Here is a paragraph</p>
</form>
```

All forms require an **action attribute**. The value of this attribute is a page that will get the client inputted information. 

This form also has a **method**. To send values with forms, a form can use two different methods, a **get** or **post**. 

---

#### Styling Tables

Empty table cells can either be show or hidden.

```css
table {
  empty-cells: hide;
}

table {
  empty-cells: show;
}
```

Remove the margin between all cells:

```css
table {
  border-collapse: collapse;
}
```

---

#### Styling Forms

Styling an input field when it ise being used:

```css
input:focus {
  background-color: #ffffff;
}
```

Vertically aligning forms through css will make them easier to use.

---

#### Events

**Events** in JavaScript are ways to signify when the user has interacted in some way with the page. A JavaScript script can then be used to respond in the appropriate manner.

**Events listeners** are used to signify this.

```javascript
elements.addEventListener('event', functionName [, Boolean]);
```



