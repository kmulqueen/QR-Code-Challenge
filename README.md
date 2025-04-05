# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - QR code component solution](#frontend-mentor---qr-code-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I Learned](#what-i-learned)
      - [Proper Semantic Structure](#proper-semantic-structure)
      - [Benefits Beyond Structure](#benefits-beyond-structure)
      - [Final Implementation](#final-implementation)
    - [Continued development](#continued-development)
    - [Useful Resources](#useful-resources)
      - [Documentation and Guides](#documentation-and-guides)
      - [Why These Resources Matter](#why-these-resources-matter)
  - [Author](#author)

## Overview

### Screenshot

![Kyle Mulqueen's desktop solution to the frontend mentor qr code challenge](./images/kyle-qr-solution-desktop.png)
_Desktop solution_

![Kyle Mulqueen's mobile solution to the frontend mentor qr code challenge](./images/kyle-qr-solution-mobile.png)
_Mobile solution_

### Links

- Solution URL: [GitHub Pages](https://kmulqueen.github.io/QR-Code-Challenge/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I Learned

This challenge significantly deepened my understanding of semantic HTML and its importance in modern web development. Key insights include:

#### Proper Semantic Structure

Initially, I avoided generic `<div>` elements but misused `<section>` tags within the QR code component. After conducting research, I implemented a more appropriate structure:

- Using `<article>` to encapsulate the self-contained QR card
- Placing the QR image within a `<figure>` element
- Implementing `<header>` for the introductory content

#### Benefits Beyond Structure

I discovered that semantic HTML delivers multiple advantages:

- **Improved accessibility** for users with screen readers and assistive technologies
- **Enhanced SEO performance** through clearer content hierarchy
- **Better document outline** for browsers and development tools
- **Future-proofing** for maintenance and scalability

#### Final Implementation

After applying these principles, my code evolved to this semantic structure:

```html
<main>
  <article class="qr-card">
    <figure>
      <img
        src="./images/image-qr-code.png"
        alt="qr code for frontendmentor.io"
        class="qr-code"
      />
    </figure>
    <header class="cta">
      <h1 class="text-preset text-bold">
        Improve your front-end skills by building projects
      </h1>
      <p class="text-preset text-regular">
        Scan the QR code to visit Frontend Mentor and take your coding skills to
        the next level
      </p>
    </header>
  </article>
</main>
```

### Continued development

This experience has reinforced the importance of thoughtful HTML structure in my development practice, a principle I'll carry forward to future projects.

### Useful Resources

#### Documentation and Guides

- [MDN - Document and Website Structure](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure) - This comprehensive guide was instrumental in helping me understand semantic HTML principles and how to structure documents for both accessibility and readability. The examples of proper sectioning content and landmark elements clarified when to use `<article>`, `<section>`, and other semantic tags.

- [MDN - Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML) - This resource provided valuable insights into the proper implementation of the `<figure>` and `<figcaption>` elements. I learned how these semantic elements enhance accessibility by providing proper context for images and allowing for more sophisticated image handling beyond basic `<img>` tags.

#### Why These Resources Matter

These MDN resources were particularly valuable because they offer both theoretical explanations and practical examples. They helped me move beyond basic HTML knowledge to implement more thoughtful, semantic markup that serves both users and search engines better.

## Author

- Website - [Kyle Mulqueen](https://kmulqueen.github.io/portfolio-2025/)
- Frontend Mentor - [@kmulqueen](https://www.frontendmentor.io/profile/kmulqueen)
