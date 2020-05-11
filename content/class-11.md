# Images || Audio & Video || SEO

---

#### Images

CSS can be used to control an image's height and width.

```css
img {
  height: 450px;
  width: 300px;
}
```

![image](https://placehold.it/450x300)

Images by default are inline elements.

**Background images** are used to act as a container but with a background image. 

```css
p {
  background-image: url("https://placehold.it/200x70");
}
```

The **background-repeat** property can have four values:

- repeat-x
- repeat-y
- repeat
- no-repeat

The **background-position** property will control where in the container the background image will be positioned.The values include:

- left top
- left center
- left bottom
- center top
- center center
- center bottom
- right top
- right center
- right bottom

These properties contain a shorthand version:

```css
body {
  background: blue url("https://placehold.it/200x70")
    no-repeat top right;
}
```

---

#### Audio & Video

Audio and video can be embedded into HTML5 by using the `<audio>` and `<video>` tags.

These elements are easy to use but often are not cross-platform compatible. They can also cus further complications.

The **HTMLMediaElement API** element allows programmers for more control over audio and video components.

```html
<div class="player">
  <video controls>
    <source src="video/sintel-short.mp4" type="video/mp4">
    <source src="video/sintel-short.webm" type="video/webm">
    <!-- fallback content here -->
  </video>
  <div class="controls">
    <button class="play" data-icon="P" aria-label="play pause toggle"></button>
    <button class="stop" data-icon="S" aria-label="stop"></button>
    <div class="timer">
      <div></div>
      <span aria-label="timer">00:00</span>
    </div>
    <button class="rwd" data-icon="B" aria-label="rewind"></button>
    <button class="fwd" data-icon="F" aria-label="fast forward"></button>
  </div>
</div>
```

Above Example taken from "https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs".

CSS is used to style everything above, and Javascript is used to implement the 'play, pause, fast-forward and rewind' aspects.

Event listeners and handlers are used to control the buttons.

---

#### SEO || Site Analytics || Deploying a website

| S      | E      | O            |
| ------ | ------ | ------------ |
| search | engine | optimization |

**Search Engine Optimization** refers to the ability to have a website appear at the top of the list in a Google search. There are both **on page techniques** and **off page techniques**.

##### **On page techniques**

There are **seven** different areas where **keywords** should be used.

- Page title
- URL / Web Address
- Headings
- Text
- Link text
- Image Alt text
- Page descriptions

##### Site Analytics

It is important to track user activity on a website to see how they were directed to the website and at which time or location on the website they decided to leave. This can help identify weak or unappealing spots in a website. Sign up for a analytics service at "https://www.google.com/analytics".

#### Deploying a website

To deploy a site, a **domain name** and **web hosting** is needed.