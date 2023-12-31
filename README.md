# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

![Screenshot of webpage with a card. There is a QR code on a blue background. Below it reads: 'Improve your front-end skills by building projects', 'Scan the QR code to visit Frontend Mentor and take your coding skills to the next level'](images\Screenshot.png)

### Links

- Solution URL: [Repo](https://github.com/halimahexe/QR-Code)
- Live Site URL: [Github.io](https://halimahexe.github.io/QR-Code)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

I felt comfortable coding the majority of this but, after watching Kevin Powell's tutorials on coding frontend projects, I decided to try out using custom CSS properties to get into the habit as I expect this will be useful when I work on bigger projects.

I learned to use `rem` for `font-size` and that it's generally preferable for accessibility to use this over `px`, so I will bear this in mind going forwards.

The main issue I had was getting Flexbox to behave correctly. Although I had a parent element `body` with a specified height, trying to get my elements to align to the centre of the webpage proved tricky. I ended up with the following code to get the right behaviour:

```css
body {
    height: 100%;
    font-family: var(--ff-sans);
    font-size: var(--fs-400);
    background-color: var(--clr-neutral-300);
}

.container {
    height: 100vh;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
```
I don't fully understand the reason that I had  to use `%` and `vh`, over using `100%` for both the `body` and `container` heights.

### Continued development

In future projects, I'd like to practise using Flexbox more, so hopefully I can be more familiar with how it works.

### Useful resources

- [CSS Tricks Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This is a really useful reference to the things you can do with Flexbox.
- [Figma](https://www.figma.com) - Although I used the free version of Frontend Mentor, so didn't have access to their Figma files, I used Figma to figure out approximate sizes of elements to get it as close as possible to the target.

## Author

- Github - [halimahexe](https://www.github.com/halimahexe)
- Frontend Mentor - [@halimahexe](https://www.frontendmentor.io/profile/halimahexe)

## Acknowledgements

Thanks to [Kevin Powell](https://www.youtube.com/@KevinPowell) for his brilliant YouTube channel with CSS tips and tricks. I decided to try out custom CSS properties because of him!