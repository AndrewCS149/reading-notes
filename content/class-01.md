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

Comments are used strictly for developer purposes. Comments are placed within `<!-- Comment goes here -->` these characters  and are not displayed to the browser. These can help with explaining complex areas within the HTML to help developers understand what is going on. 

#### iframe element

The `<iframe>` element is used to embed a smaller window with another page inside of it. The iframe element uses the following attributes:

- `width="450"`
- `height="350"`
- `src="linkToPage"`

<iframe
    width="450"
    height="350"
    src="https://www.codefellows.org/">
</iframe>

#### HTML5 Layout

`<header>` and `<footer>` elements are placed along the top and bottom of every page. Typically, the header element will contain the site name and the main navigation bar, which is used with the `<nav>` tag. The nav tag will hold links to other pages of the website, such as a 'products' page or a 'contact' page. The footer tag usually holds the copyright information. 

The `<section>` tag is used to group together related content to help CSS style the entire related section at once. 

The `<div>` element is quite similar to the section tag. The div tag should be used when there is no other suitable option to group together material. Older versions of HTML used the div tag much more often. 

#### Process & Design

Before punching out a bunch of HTML into a page, it is best practice to first create a basic idea of what your site is going to be about. To better understand how your website is going to be layed out, ask yourself these questions:

- *Who is this site for?*
- *Why will people come to this site?*
- *What are people trying to accomplish on this site?*
- *How frequently will people come to this site?*

Once you have a basic understanding of what your desired website will need to contain, then create a **wireframe**. Essentially, a wireframe is a drawing of what the website will look like. Wireframs *should* include structural information and *should not* include aesthetic information, such as font, color, etc.

---

### JavaScript

#### What is a Script?

A **script** is a set of instructions that is given to the computer to complete a very specific task. Consider the following instructions to make a bed:

1. Get out of bed.
2. Pull bottom-left corner of blanket over bottom-left corner of mattress. 
3. Pull bottom-right corner of blanket over bottom-right corner of mattress. 
4. Pull top-right corner of blanket over top-right corner of mattress. 
5. Pull top-left corner of blanket over top-left corner of mattress. 
6. Fluff pillows.
7. Put pillows against the bed frame. 

Obviously, we don't need to specify to someone exactly how to make a bed, but this is a good example of how specific we need to be to tell a computer to do something. To begin making a script, a goal must first be discovered. Then, a list of instructions need to be stated in order to reach the given goal.  

#### Objects and Properties 

Think of a hotel as an object. This object can have many different properties and the properties will each contain a value. 

| properties      | values |
| --------------- | ------ |
| name            | Hilton |
| rating          | 4      |
| rooms           | 200    |
| rooms available | 20     |
| rooms booked    | 180    |
| gym             | true   |
| pool            | false  |

A car can be thought of as the same way. 

| properties       | values |
| ---------------- | ------ |
| make             | Honda  |
| model            | civic  |
| color            | white  |
| year             | 2017   |
| body type        | sedan  |
| MPG avg          | 34.5   |
| leather interior | true   |
| current speed    | 50     |

Everything is an object, and all objects have properties. A web page is made up of objects and properties as well.

#### Events 

An **event** is an interaction with an object. Think back to the car example. When the gas pedal is pressed, the car accelerates. When the brake pedal is pressed, the car slows down. These are examples of events. Something needs to happen in order for these events to occur, *ig* 'gas pedal is pressed' and 'brake pedal is pressed'. 

#### Methods 

A **method** is essentially a change or an update to an object property value. Looking again back to the car example, a method named `changeSpeed()` could be used to increase or decrease the speed of the car. This method will contain instructions, or a **script**, to carry out the command to change the speed. 

The other example, Hilton hotel, would also need many different methods, such as `makeBooking()`, `cancelBooking()` or `checkAvailability()`. 

#### Putting Everything together

All of the above topics can be combined to make a computer program work. Here is how the car object would work:

1. Driver presses gas pedal and the 'accelerator event' triggers
2. The accelerator event calls the `changeSpeed()` method which then increases the current speed of the car. 
3. The `current speed` property now holds the value that was changed by the `changeSpeed()` method. 

Just like the above examples, computer programs are comprised of objects, methods and events. The HTML page is a document object and the window is a window object. 

---

### HTML, CSS & JavaScript Working Together 

Imagine that HTML, CSS and JavaScript are all separate layers. HTML is the **content** layer, CSS is the **presentation** layer and JavaScript is the **Behavior** layer. 

1. HTML - content
2. CSS - presentation 
3. JavaScript - behavior 

HTML is the text, or content of a page. CSS is how that content is displayed on the page, and JavaScript is how that page can be interacted with, such as buttons, animations and such. 