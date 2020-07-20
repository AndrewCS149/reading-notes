# Intro To MVC

| M     | V    | C          |
| ----- | ---- | ---------- |
| Model | View | Controller |

The MVC is a popular framework for creating web apps and API's. This approach helps with separation of concerns.

*What is separation of concerns?*

This refers to keeping separating software depending on the type of functionality it contains. This can help with updating a script without having to revamp the entirety of it.

---

### Model 

The *model* is where the meat of the application exists. This performs the logic and the actual application functionality. 

---

### View 

The *view* is responsible for presenting the user with content. This is accomplished with the **Razor view engine**, which we will get into later. The view should contain minimal amounts of logic and leave that to be handles by the controller. Essentially, the view simply displays information to the user. 

---

### Controller

The *controller* responds to the user input and handles all the user interaction. 

---

### ASP.NET Core MVC

The *ASP.NET Core MVC framework* is lightweight  framework that is used with ASP.NET Core. It includes the following functionality:

- [x] Routing
- [x] Model binding
- [x] Model validation
- [x] Dependency injection
- [x] Filter
- [x] Areas
- [x] Web APIs
- [x] Testability 
- [x] Razor view engine
- [x] Strongly typed views
- [x] Tag Helpers
- [x] View components 

---

### Razor View Engine

As mentioned above, the *Razor view engine* is used to display content to the user through an HTML page. This is very similar that of *ejs*. 

Example:

```html
<ul>
  @for (int i = 0; i < 10; i++) 
  {
    <li> List Item:@i</li>
  }
</ul>
```

