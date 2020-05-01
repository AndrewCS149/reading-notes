# HTML Images || CSS Color & Text

---

#### Images

HTML uses the `<img>` tag to embed photos to a website. This can make a site feel much more welcoming. It is important to note that using an image downloaded from another website will have negative repercussions, so make sure to acquire those images through a photo stock website.

The `<img>` tag requires the `src` attribute to give the correct path to the image. The `alt` attribute can optionally be placed in the `<img>` tag to display some text in case the image does not load property.

`<img src="example/dog.jpg" alt="A picture of a dog"/>`

The height and width can be controlled through html as well in pixels.

`<img src="example/dog.jpg" alt="A picture of a dog" width="500" height="350"/>`

The `<figure>` element is used to wrap around an `<img>` tag. After the image tag, place a `<figcaption>` element with a brief caption describing the image. This was implemented as a new element to HTML5.

```html
<figure>
  <img src="example/dog.jpg" alt="A picture of a dog" width="500" height="350"/>
  <br/>
  <figcaption>A dog running after a ball</figcaption>
</figure>
```


**Image formats**
Use the JPEG format when saving an image with a lot of color.
Use GIF or PNG formatting when saving an image with no color or images that are filled with primarily the same color.

---

#### Color

Every computer color is a mixture of **red, green, and blue** values. These values range from **0-255**. Color names can be specified in three different ways:
* **RGB values** - `rgb(50, 200, 40)`
* **Hex Codes** - ` #22rdlb`
* **Color Name** - `red, cyan, steelblue` 

CSS3 also allows for specifying colors with **HSL** values. 

| H   | S          | L         |
| --- | ---------- | --------- |
| hue | saturation | lightness |

An additional property can be appended to this, HSL**A**. The A is for alpha which refers to the color transparency.

---

#### Text

When changing fonts with CSS, it is important to note that not all computers may have a specific font stored in their memory, therefor it will not be displayed. Because of this, a generic font should be placed AFTER the desired font (in the case the the computer doesn't have that font installed).

* serif
* sans-serif
* monospace
* cursive
* fantasy

Font type is specified with the `font-family:` property, while the size uses the `font-size:` property. The default size of a browser's text is **16px**. Different font size can be achieved through **pixels**, **percentages** and **ems**. Below is a table that shows scaling options between all three of these options.

**| 12 PIXEL SCALE |**
| tag  | PIXELS | PERCENTAGES | EMs    |
| ---- | ------ | ----------- | ------ |
| h1   | 24px   | 200%        | 1.5em  |
| h2   | 18px   | 150%        | 1.3em  |
| h3   | 14px   | 117%        | 1.17em |
| body | 12px   | 75%         | 100%   |
| p    |        |             | 0.75em |

**| 16 PIXEL SCALE |**
| tag  | PIXELS | PERCENTAGES | EMs     |
| ---- | ------ | ----------- | ------- |
| h1   | 32px   | 200%        | 2em     |
| h2   | 24px   | 150%        | 1.5em   |
| h3   | 18px   | 133%        | 1.125em |
| body | 16px   | 100%        | 100%    |
| p    |        |             | 1em     |

Ems size is based off of it's parent element.

The `verticle-align:` property will allow the text to move to the desired position within it's box boundaries. Values can include `text-top; text-bottom; baseline`.

Pseudo classes are used to change the appearance of an element when the user has interacted with that element such as hovering or visiting a link. When using pseudo-classes, it is important to style them with in this order:

```css
a:link
a:visited
a:hover
a:focus
a:active
```