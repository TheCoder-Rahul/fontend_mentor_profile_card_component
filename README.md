# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![Design screenshot](https://github.com/TheCoder-Rahul/fontend_mentor_profile_card_component/blob/main/project_screenshot.png)

### Links

- 👉 [Solution URL](https://github.com/TheCoder-Rahul/fontend_mentor_profile_card_component.git)
- 👉 [Live Site URL](https://thecoder-rahul.github.io/fontend_mentor_profile_card_component/)

## My process

### Built with

- 👉 **Markup:** Semantic HTML5 for better accessibility and SEO.
- 👉 **Styling:** CSS3 with Custom Properties (variables) for a maintainable color scheme, font-properties, and different sizes.
- 👉 **Layout:** Flexbox for centering the card and managing the internal alignment.
- 👉 **Workflow:** Mobile-first approach and Responsive Design using Media Queries.

### What I learned

Check the code snippets attached below:

```html
<main>
  <img class="bg_top" src="./images/bg-pattern-top.svg" alt="Body Background Pattern Image">
  <article>
    <img class="img crd_bg_ptrn" src="./images/bg-pattern-card.svg" alt="Profile Card Background Pattern">
    <section class="prof_dtls">
      <img class="img usr_pic" src="./images/image-victor.jpg" alt="Victor Crest Profile Picture">
      <h1>Victor Crest <span>26</span></h1>
      <p>London</p>
      <hr>
      <section class="metrics">
        <div class="flwrs">
          <h2>80K</h2>
          <p>Followers</p>
        </div>
        <div class="likes">
          <h2>803K</h2>
          <p>Likes</h2>
        </div>
        <div class="photos">
          <h2>1.4K</h2>
          <p>Photos</h2>
        </div>
      </section>
    </section>
  </article>
  <img class="bg_btm" src="./images/bg-pattern-top.svg" alt="Body Background Pattern Image">
</main>
```
```css
*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root {
  --blue-600: hsl(185, 75%, 39%);
  --navy-950: hsl(229, 23%, 23%);
  --gray-500: hsl(227, 10%, 46%);
  --gray-100: hsl(225, 10%, 92%);
  --navy-950_20: hsla(229, 23%, 23%, 0.2);
  --body-font: "Kumbh Sans", sans-serif;
}
body {
  font-size: 1.125rem;
  color: var(--gray-500);
  font-family: var(--body-font);
  background-color: var(--blue-600);
}
.img {
  height: auto;
  display: block;
  max-width: 100%;
}
main {
  display: flex;
  height: 100vh;
  overflow: hidden;
  position: relative;
  align-items: center;
  justify-content: center;
}
.bg_top, .bg_btm {
  z-index: -1;
  position: absolute;
}
.bg_top {
  inset: 0 auto auto 0;
  transform: translate(-75%, -60%);
}
.bg_btm {
  inset: auto 0 0 auto;
  transform: translate(65%, 65%);
}
article {
  overflow: hidden;
  border-radius: 1rem;
  margin-inline: 1.5rem;
  background-color: var(--gray-100);
  box-shadow: 0 2rem 2rem var(--navy-950_20);
}
.prof_dtls {
  text-align: center;
}
.prof_dtls .usr_pic {
  margin: 0 auto;
  border-radius: 50%;
  margin-block-end: -8%;
  transform: translateY(-50%);
  border: 0.3125rem solid var(--gray-100);
}
.prof_dtls h1, .prof_dtls .metrics h2 {
  font-size: 1.125rem;
  color: var(--navy-950);
  margin-block-end: 0.25rem;
}
.prof_dtls h1 span {
  font-weight: 400;
  color: var(--gray-500);
  margin-inline-start: 0.25rem;
}
.prof_dtls p {
  font-size: 0.9375rem;
}
.prof_dtls hr {
  opacity: 0.2;
  margin: 1.5rem 0;
}
.prof_dtls .metrics {
  display: flex;
  align-items: center;
  padding-block-end: 1.5rem;
  justify-content: space-evenly;
}
.prof_dtls .metrics h2 {
  margin-block-end: 0;
}
.prof_dtls .metrics p {
  font-size: 0.75rem;
  letter-spacing: 1px;
}
.attribution { font-size: 0.6875rem; color: var(--gray-100); text-align: center; position: absolute; inset: auto 0 0.25rem; }
.attribution a { color: var(--navy-950); }
@media (min-width: 48rem) {
  article {
    margin-inline: 0;
  }
}
```

## Author

- 👉 GitHub - [TheCoder-Rahul](https://github.com/TheCoder-Rahul)
- 👉 Frontend Mentor - [@TheCoder-Rahul](https://www.frontendmentor.io/profile/TheCoder-Rahul)
- 👉 LinkedIn - [@Rahul Kumar](https://www.linkedin.com/in/rahul-the-developer/)