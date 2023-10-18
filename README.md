# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

  - [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
  - [Author](#author)


## Overview

NFT preview card component challenge by Frontend Mentor 

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned

I have learned about combining absolute position on the  image container with div inside of it holding svg element with background in order to make hover effect on the image. 
<!--  Code -->
.image-container{
    position: relative;
    max-width: 22rem;
    border-radius: 1rem;
    overflow: hidden;
}
.nft{
    object-fit: cover;
    object-position: center;
}
.content{
    position: absolute;
    inset: 0;
    display: grid;
    place-content: center;
    background-color: var(--clr-cyan);
}

.nft,
.content{
    transition: .4s ease-in-out;
}

.content.accent{
    opacity: 0;
}
.content:hover.accent{
    opacity: .6;
}
<!--  -->

### Useful resources

This is very useful video on hover effects that helped me understand how i could  implement it in my challenge - https://www.youtube.com/watch?v=tF3RE5CGt9U and who channel WebDevSimplified in general

Not related specificaly to this project but something i wanted to understand since i was using grid in this project and its properties and here is the video on difference between Grids Place-content and place-items https://www.youtube.com/watch?v=vNwoDkn7AIc

## Author

- Github - https://github.com/nenadvg95?tab=repositories
- Frontend Mentor - https://www.frontendmentor.io/profile/nenadvg95

