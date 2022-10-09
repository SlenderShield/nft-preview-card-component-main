# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![Screen Shot](./images/preview%20card%20component.png)

### Links

- Solution URL: [Frontend Mentor](https://www.frontendmentor.io/solutions/responsive-nft-card-built-using-css-flexbox-CIHwT1zHHf)
- Live Site URL: [nft-preview-card-component-main](https://slendershield.github.io/nft-preview-card-component-main)

## My process

### Built with

- Semantic HTML5 markup
- CSS basics
- CSS Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

The hardest topic to understand was the overlaying a image over another image on active state.
Through this challenge i left how to do it and the understood the concept a bit more.

To see how you can add code snippets, see below:

```html
<div class="container">
	<img
		src="./images/image-equilibrium.jpg"
		alt="image of nft"
		class="nft-img"
	/>
	<div class="overlay">
		<img src="./images/icon-view.svg" alt="icon" />
	</div>
</div>
```

```css
.container {
	position: relative;
}

.nft-img {
	opacity: 1;
	width: 260px;
	height: 260px;
	border-radius: 10px;
	display: block;
	transition: 0.5 ease;
}
.overlay {
	transition: 0.5s ease;
	opacity: 0;
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
	text-align: center;
}

.container:hover .nft-img {
	opacity: 0.5;
}

.container:hover .overlay {
	opacity: 1;
}
```

### Continued development

CSS is a vast topic to cover. I want to get more in-depth knowledge in css properties and its use cases.

### Useful resources

- [W3 Schools](https://www.w3schools.com/howto/howto_css_image_overlay.asp) - This helped me for image overlay reason. I really liked this pattern and will use it going forward.

## Author

- Website - [Muralidhara Bhat KS](https://muralidharabhat.me)
- Frontend Mentor - [@SlenderShield](https://www.frontendmentor.io/profile/SlenderShield)
- Twitter - [@myself_MDB](https://www.twitter.com/myself_MDB)

## Acknowledgments

I want to thank W3 Schools for their explanation with examples of the css properties and their use.
