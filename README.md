# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Desktop-first workflow
- CSS @media Rule


### What I learned

- To prevent clickable area to overflow the text area, I used <div> to block this effect.

```html
<div class="change">
  <a href="#" title="Change your Plan" id="change">Change</a>
</div>
```

- To change the border radius of the top image according to the whole element I used:

```css
.bubble {
  border-radius: 2em;
  overflow: hidden;
}
```

- To prevent text from wrapping:

```css
h2 {
  white-space: nowrap;
}
```

- To organize plan box I used CSS Grid with template areas:

```css
.plan-box {
  display: grid;
  grid-template-areas:
    "music text change"
    "music text change";
  grid-template-columns: 1fr 1fr 2fr;
  place-items: center right;
}
```

- To change the gap between "Annual Plan" and the price:

```css
.plan-text > * {
  margin: 1em .5em;
}
```

- To make the transition into hover state look nicer:

```css
a {
  transition: all .2s ease-in;
}
```

To adjust the design for mobile devices I mostly used em, rem and % and change ratio via @media queries:

```css
@media only screen and (max-width: 480px) {
  :root {
    font: 8px/25px 'Red Hat Display', sans-serif;
  }
}
```

### Continued development

In my future projects I plan to focus on Responsiveness of a website, possibly implementing Bootstrap. I would also want to exercise the use of grid and flexbox as concerns CSS.

### Useful resources

- [CSS Tricks](https://css-tricks.com) - This helped me understand which technology between Grid and Flexbox would be easier to implement in my project.
