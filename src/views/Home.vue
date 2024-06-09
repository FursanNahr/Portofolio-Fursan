<template>
  <!-- HEADER -->
  <header class="header" id="header">
    <nav class="nav container">
      <a href="" class="nav__logo">Ukur</a>
      <div class="nav__menu" id="nav-menu">
        <ul class="nav__list">
          <li>
            <a href="#home" class="nav__link">Home</a>
          </li>
          <li>
            <a href="#work" class="nav__link">Work</a>
          </li>
          <li>
            <a href="#info" class="nav__link">Info</a>
          </li>
          <li>
            <a href="#service" class="nav__link">Services</a>
          </li>
          <li>
            <a href="#contact" class="nav__link">Contact</a>
          </li>
        </ul>

        <!-- Close button -->
        <div class="nav__close" id="nav-close">

        </div>

        <!-- Toggle button -->
         <div class="toggle__button" id="toggle-button">

         </div>
      </div>
    </nav>
  </header>

  <main></main>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400..800&display=swap');
/* Variable CSS */
:root {
  --header-height: 3.5rem;

  /* Colors */
  --hue: 230;
  --first-color: hsl(var(--hue), 55%, 55%);
  --first-color-light: hsl(var(--hue), 55%, 65%);
  --first-color-alt: hsl(var(--hue), 50%, 50%);
  --title-color: hsl(var(--hue), 30%, 95%);
  --text-color: hsl(var(--hue), 20%, 80%);
  --text-color-light: hsl(var(--hue), 20%, 70%);
  --body-color: hsl(var(--hue), 40%, 16%);
  --container-color: hsl(var(--hue), 40%, 20%);

  /* Font and Typography */
  /* .5rem = 8px | 1rem = 16px */
  --body-font: "Syne", sans-serif;
  --biggest-font-size: 3rem;
  --big-font-size: 1.5rem;
  --h1-font-size: 1.5rem;
  --h2-font-size: 1.25rem;
  --h3-font-size: 1rem;
  --normal-font-size: .938rem;
  --samll-font-size: .813rem;

  /* Font Weight */
  --font-regular: 400;
  --font-semi-bold: 600;
  --font-bold: 700;

/* Z Index */
--z-tooltip: 10;
--z-fixed: 100;
}

@media screen and (min-width: 1550px) {
  :root {
    --biggest-font-size: 5.5rem;
    --big-font-size: 2.75rem;
    --h1-font-size: 2.25rem;
    --h2-font-size: 1.5rem;
    --h3-font-size: 1.25rem;
    --normal-font-size: 1.125rem;
    --small-font-size: .875rem;
  }
}

/* Base */
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

html {
  scroll-behavior: smooth;
}

body,
input,
textarea,
button {
  font-family: var(--body-font);
  font-size: var(--normal-font-size);
}

body {
  background-color: var(--body-color);
  color: var(--text-color);
}

input,
button,
textarea {
  border: none;
  outline: none;
}

h1, h2, h3 {
  color: var(--title-color);
  font-weight: var(--font-semi-bold);
}

p {
  line-height: 130%;
}

ul {
  list-style: none;
}
a {
  text-decoration: none;
}

img {
  display: block;
  max-width: 100%;
  height: auto;
}

/* Reusable CSS Class */
.container {
  max-width: 1120px;
  margin-inline: 1.5rem;
}

.grid {
  display: grid;
  gap: 1.5rem;
}

/* Header & Nav */
.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: transparent;
  z-index: var(--z-fixed);
}
.nav {
  position: relative;
  height: var(--header-height);
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.nav__logo {
  color: var(--title-color);
  font-weight: var(--font-bold);
}

</style>
