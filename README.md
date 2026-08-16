# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Links

- Solution URL: [GitHub Repository](https://github.com/marek-milacek/frontendmentor-testimonials-grid-section)
- Live Site URL: [GitHub Pages Live Demo](https://marek-milacek.github.io/frontendmentor-testimonials-grid-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (variables)
- Mobile-first workflow
- CSS Grid (`grid-template-columns`, `grid-template-rows`, `grid-area`)
- Flexbox

### What I learned

During this project, I deepened my understanding of:
1. **CSS Grid Placement**: Using `grid-area` to position complex card layouts across multiple columns and rows.
2. **Responsive Breakpoint Strategy**: Applying a Mobile-First workflow with `@media (min-width: 950px)` to transition smoothly from a single-column layout on mobile devices to a 4-column grid layout on desktop.
3. **Container-level Constraints vs Card Constraints**: Setting `max-width` on the `.grid-container` and resetting `max-width: none` on individual cards for desktop view so cards span across grid tracks properly.
4. **CSS Background Decoration**: Using `background-image`, `background-repeat`, and `background-position` for decorative SVG icons behind card text.

```css
.daniel {
    background-image: url("./images/bg-pattern-quotation.svg");
    background-repeat: no-repeat;
    background-position: top right 80px;
}

@media (min-width: 950px) {
    .grid-container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(2, 1fr);
        max-width: 1100px;
        gap: 20px;
    }

    .daniel {
        grid-area: 1 / 1 / 2 / 3;
    }
}
```

## Author

- Frontend Mentor - [@marek-milacek](https://www.frontendmentor.io/profile/marek-milacek)
- GitHub - [@marek-milacek](https://github.com/marek-milacek)
