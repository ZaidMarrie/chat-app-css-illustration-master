# Frontend Mentor - Chat app CSS illustration solution

This is a solution to the [Chat app CSS illustration challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/chat-app-css-illustration-O5auMkFqY). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- **Bonus**: See the chat interface animate on the initial load

### Screenshot



### Links

- [My Solution](https://your-solution-url.com)
- [Live Site Demo](https://zaidmarrie.github.io/chat-app-css-illustration-master/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Completing this challenge was fun. I learnt how to create custom radio buttons/input. This I accomplished using psuedo elements.

To see how you can add code snippets, see below:

```html
<label for="opt-1" class="radio-label">
    <input type="radio" name="walk" id="opt-1" class="radio-btn">
    <div class="radio"></div>
    30 minute walk<span class="price">$29</span>
</label>
```
```css
.radio-label{
    display: inline-flex;
    align-items: center;
}

.radio{
    width: 1.125em;
    height: 1.125em;
    padding: 2px;
    margin-right: .5em;
    border-radius: 50%;
    border: 3px solid var(--secondary-radio-outline);
    background: transparent;
    position: relative;
}
```
```css
.radio::after{
    content: '';
    width: 100%;
    height: 100%;
    background: #ffffff;
    border-radius: 50%;
    position: absolute;
    top: 0;
    left: 0;
    transform: scale(0);
    transition: transform 250ms;
}

.radio-btn:checked ~ .radio::after{
    transform: scale(1);
}
```

### Useful resources

[W3schools](https://www.w3schools.com/howto/howto_css_custom_checkbox.asp) This helped me create a custom radio button

## Author

- Frontend Mentor - [@ZaidMarrie](https://www.frontendmentor.io/profile/ZaidMarrie)
- Twitter - [@LeKoels27](https://twitter.com/LeKoels27)
