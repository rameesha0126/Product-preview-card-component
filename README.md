# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Product preview card component solution](#frontend-mentor---product-preview-card-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
    - [Useful resources](#useful-resources)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

[Mobile Design](Mobile-view.png)
[Desktop Design](Desktop-view.png)

### Links

- Solution URL: [solution](https://your-solution-url.com)
- Live Site URL: [Live Site](https://rameesha0126.github.io/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Media Queries

### What I learned

When using flexbox, use "Align-items" and "Justify-content" properties to perfectly center an object within the viewport. 
Using "width: 100%" will change the absolute width according to the screensize. Set max-width to provide an upper limit to the width.

Use below mentioned code to change the image file used when the screensize is at a certain value. when the width is more than 376px first image gile is used, when it's less the second image file is used. This corresponds with the flex display we have used.
```html
<picture>
  <source media="(min-width: 376px)" srcset="images\image-product-desktop.jpg">
  <img src="images\image-product-mobile.jpg" alt="Perfume bottle">
</picture>
```
Flex display for mobile screen width.
```css
@media only screen and (max-width: 375px) {
    .Preview-card-element {
        display: flex;
        flex-direction: column;
        min-height: 100vh;
        min-width: 90vw;
        margin: 2em 1em;
    }
}
```

### Continued development

Conforming to the given image sizes and layouts when changing the display size. 

### Useful resources

- [W3schools CSS Tutorial](https://www.w3schools.com/css/default.asp)

## Author

- Github - [Rameesha0126](https://github.com/rameesha0126)
- Frontend Mentor - [@rameesha0126](https://www.frontendmentor.io/profile/rameesha0126)
