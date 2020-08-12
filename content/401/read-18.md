# Layouts 

### What are Layouts?

A layout is a web design or format that carries from page to page in a web application. This allows users to know how to navigate seamlessly between pages. 

The most common layouts that are consistent through an entire application are:
- Header
- Footer
- Navigation
- Menu

Plenty of html and css pages are used by all pages. If a css style or html format is expected to be the same between every page, it would be a good idea to put inside of a 'Shared' folder within the 'Pages' folder. 

To use the html file from within the the 'Shared' folder, import into the current html doc like so:

```csharp
@ {
  Layout = "_Layout";
}
```
---

### Partial Views

Partial views are useful for breaking up large files into sections. 

Partial views are essentially html (or css) components that are inserted into another html file. 

Partial views are commonly used with things that stay consistent over the entire page, such as: 
- Header
- Footer
- Nav
- Menu

