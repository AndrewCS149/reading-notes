# jQuery || Paired Programming

JQuery is a JavaScript library that allows for much easier access to html elements. It also makes manipulating the DOM, changing css and using attaching handlers much easier.

Selecting by tag name:

```js
$('div');
```

Selecting by ID:


```js
$('#main-hav');
```

Selecting by class name:

```js
$('.nav');
```

Adding a class:

```js
$('nav').addClass('main-nav');
```

The `.ready` function ensures that the page is ready before executing the JavaScript.

```js
$(document).ready(function() {
  // code goes here
});
```

Shortcut version: 

```js
$(function() {
  // code goes here
})
```

Adding elements to the page:

```js
.before()
.after()
.prepend()
.append()
```

Getters and Setters:

```js
$('li').text();
$('li').text('hello world!');
```

Getting  and setting a css property:

```js
var backgroundColor = $('li').css('background-color');
$('li').css('background-color', 'blue');
```

Events:

```js
$('#form')(.submit(function(){
  // code goes here
}))
```

```js
$('li').on('click', function() {
  $(this).addClass('complete');
})
```

Ajax:
1. Get the data.
2. Tell what type of data and what format the data is in.
3. Then, tell what to do with the data.
 
```js
$.ajax('/filpath');

$.ajax('/filepath', {method: "GET", dataType: "JSON"});

$.ajax('filepath', {method: "GET", datType: "JSON"});
.then(data=>// do something)
```

**Ways** to implement jQuery:

* CDN (Content Delivery Network)
* As another file in your directory

**Where** to put the jQuery

* Before the closing `</head>` tag
* Inside the page
* Before the closing `</body>` tag

---

### Paired Programming

**Benefits**

 * Better Collaboration
 * More Efficient
 * Learn from others
 * Improve social skills
 * Prepare for interviews
 * Create work-ready individuals