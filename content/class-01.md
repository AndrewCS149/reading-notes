# HTML | CSS | JavaScript

---

### HTML

What is HTML? HTML is the *language* that is used to structure all web pages on the internet. 

| H     | T    | M      | L        |
| ----- | ---- | ------ | -------- |
| hyper | text | markup | language |

HTML uses **elements**, or **tags**, to give the content within the page different meaning and importance. These elements consist of opening tags and closing tags and act like containers. The content that is between the opening and closing tags belongs to that element. 

Here are some examples:

- `<h1> Header 1 </h1>`
- `<h2> Header 2 </h2>`
- `<p> Paragraph </p>`
- `<header> Header </header>`
- `<footer> Footer </footer>`
- `<main> Main </main>`

| `<h1>`        | `Header 1`         | `</h1>`       |
| ------------- | ------------------ | ------------- |
| `opening tag` | `targeted content` | `closing tag` |

#### Attributes 

**Attributes** are placed inside the elements opening tag and give more information about that element. Attributes are optional and some elements may even contain more than one attribute. 
Example: 

`<p lang="en-us"> English paragraph.</p>`

| attribute | attribute value |
| :-------: | :-------------: |
|  `lang`   |    `"en-us"`    |

The attribute in this case signifies that the paragraph is in English. 
The **ID** and **Class** attributes are used to give the element a way to be accessed from CSS (which we will get into later on). 
Example:

`<p id="tolkienQuote">“All we have to decide is what to do with the time that is given us.” - J.R.R. Tolkien, The Lord of the Rings</p>`


`<p class="quotes">“Even the smallest person can change the course of the future.”- J.R.R. Tolkien, The Lord of the Rings</p>`

The difference between the id and class attribute is that the id attribute is one, **unique** value different from any other id or class attribute on the page, but the class attribute value can have **one or more** elements with the exact same value. 

#### Different HTML Versions

Since there have been several versions of HTML released, we need to specify which version the browser which version of HTML is being used. Currently, HTML5 is being used. We do this with the `<!DOCTYPE html>` element. This tag must come before any other element. 

#### Comments 

**Comments** are used strictly for developer purposes. Comments are placed within `<!-- Comment goes here -->` these characters  and are not displayed to the browser. These can help with explaining complex areas within the HTML to help developers understand what is going on. 

#### iframe element

<iframe
    width="450"
    height="350"
    src="https://www.google.com/maps/place/Code+Fellows/@47.6183043,-122.3530041,17z/data=!4m12!1m6!3m5!1s0x5490153758c88a61:0xe3d3fd29c55db518!2sCode+Fellows!8m2!3d47.6183694!4d-122.3517917!3m4!1s0x5490153758c88a61:0xe3d3fd29c55db518!8m2!3d47.6183694!4d-122.3517917
    &amp;output=embed">
</iframe>






---

### CSS

---

### JavaScript