# Responsive Web Design || FLoats || SMACSS

---

### RWD (responsive web design)

RWD is the process of creating a website that works seamlessly between all devices with all screen sizes.

RWD can be compartmentalized into three subcategories: **Flexible Layouts, Media Queries,** and **Flexible Media.** 

#### Flexible Layouts

Relative units that are commonly used amongst flexible layouts:

* vw - viewport width
* vh - viewport height
* vmin - minimum of the vh and vw
* vmax - maximum of the vh and vw

In order to achieve a flexible layout, it is best to avoid using unit sizes such as pixels. Here is an accurate formula for determining a good proportionate size of a flexible layout. 

**target / context = result**

#### Media Queries

There are three ways to use a media query:

1. Using the @import
2. Linking to a separate style sheet from the HTML
3. Using @media queries within the same stylesheet

The third option is best practice. 

Logical operators (and, not and only) are available to use within media queries.

```css
@media all and (min-width: 800px) and (max-width: 1024px) {

  /* code goes here */

}
```

Setting max and min height and width properties is a large proprietor in using media queries. The height and width properties are based off of the viewport height and width.

The **orientation** media feature is used to figure out if the user is in landscape or portrait mode.

```css
@media all and (orientation: landscape) {

  /* code goes here */

}
```

**Aspect Ratio** media queries set the minimum or maximum given aspect ratio.

```css
@media all and (min-device-aspect-ration: 16:9) {

  /* code goes here */

}
```

**Resolution media queries** set the resolution in pixel density, or **dots per inch** (DPI). These queries DO NOT accept min and max prefixes. 

```css
@media print and (min-resolution: 300dpi) {

  /* code goes here */

}
```

Here is a complete media queries example:

```css
@media all and (max-width: 420px) {
  section, aside {
    float: none;
    width: auto;
  }
}
```

An effective technique in building responsive web designs is using the **Mobile First** approach. This entails configuring a design that will first apply to smaller device viewports and using the media queries to adjust those sizes to larger device. The popularity of this approach is due to the fact that the majority of the world is using mobile devices far more than desktop applications, so it makes sense to first configure an application tailored to mobile devices. Obviously, this approach should not be applied to building applications that WILL NOT be used via mobile. 

The **html meta tag** is used to inherit the user's device viewport width (or height).

```html
<meta name="viewport" content="width=device-width">
```

The content attribute can also accept a scale value that will set the initial scale based on the user's viewport. 

```html
<meta name="viewport" content="initial-scale=2">
```

We can also insert a meta tag to enable scaling (zooming).

```html
<meta name="viewport" content="minimum-scale=0">
<meta name="viewport" content="user-scalable=yes">
```

DO NOT set the minimum-scale value to the same value as the initial-scale. This will DISABLE any scaling (zooming).

#### Flexible Media

Flexible media refers to any type of media that is applied to a page, such as images or videos. Often times, these do not scale with the rest of the page, causing ugly designs after scaling is applied.

A quick remedy is to set the max-width of the media to 100%. This will allow it to shrink as the viewport gets smaller.

```css
img, video {
  max-width: 100%;
}
```

This method DOES NOT work with embedded media, such as iframes. To scale embedded media, the embedded element needs to have an absolute position inside of a containing element. The containing or parent element needs to have a width of 100%.

```html
<figure>
  <iframe src="https://videoExample.com"></iframe>
</figure>
```

```css
figure {
  height: 0;
  position: relative;
  width: 100%;
}
iframe {
  height: 100%;
  left: 0;
  position: absolute;
  top: 0;
  width: 100%;
}
```

---

### Floats

FLoating an element allows surrounding text to essentially **wrap** around the floated element. Elements can be floated either **left** or **right**. 

```css
div {
  float: left;
}
```

There are much more effective and problem free ways of creating similar layouts, such as **flexbox** or **grid**. 

The **clear** property will allow an element following a floated element to not wrap around the floated element. 

---

### SMACSS | Scalable and Modular Architecture for CSS

SMACSS Rules: 

1. Base
   1. Applies to element selector
   2. Does not include class or Id selectors
   3. CSS Reset
2. Layout
   1. Defines layout values such as height, width, or margin
   2. Normally has a single selector: either a class or id
3. Module
   1. Includes navigation, carousels, dialogs, widgets and more.
   2. Sit inside of layout components
   3. Avoid using Id selectors and element selectors
   4. Stick to class selectors
4. State
   1. Over-rides all other styles
   2. Normally applied as a layout rule or selecting the same tag as a module class
   3. State styles require JavaScript to over ride the module
5. Theme
   1. The visual appeal to the page such as colors
   2. Can override other styles

