<template>
  <!-- RemixIcon -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/remixicon/4.2.0/remixicon.min.css"
    integrity="sha512-MqL4+Io386IOPMKKyplKII0pVW5e+kb+PI/I3N87G3fHIfrgNNsRpzIXEi+0MQC0sR9xZNqZqCYVcC61fL5+Vg=="
    crossorigin="anonymous" referrerpolicy="no-referrer" />

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
          <i class="ri-close-large-line"></i>
        </div>
      </div>
      <!-- Toggle button -->
      <div class="nav__toggle" id="nav-toggle">
        <i class="ri-menu-line"></i>
      </div>
    </nav>
  </header>

  <main>
    <section class="home section" id="home">
      <div class="home__container container grid">
        <img src="../assets/images/fotoukur.png" alt="" class="home__img">

        <div class="home__data">
          <h1 class="home__name">Fursan <br> Nahr</h1>
          <h3 class="home__profession">Web Developer</h3>
        </div>

        <a href="#work" class="home__scroll">
          <div class="home__scroll-box">
            <i class="ri-arrow-down-line"></i>
          </div>

          <span class="home__scroll-text">Recent Works</span>
        </a>
      </div>
    </section>
    <section class="work section" id="work">

    </section>
    <section class="info section" id="info">

    </section>
  </main>
</template>
<script>
export default {
  mounted() {
    const navMenu = document.getElementById('nav-menu');
    const navToggle = document.getElementById('nav-toggle');
    const navClose = document.getElementById('nav-close');

    // Show Menu
    if (navToggle) {
      navToggle.addEventListener('click', () => {
        navMenu.classList.add('show-menu');
      });
    }

    // Close Menu
    if (navClose) {
      navClose.addEventListener('click', () => {
        navMenu.classList.remove('show-menu');
      });
    }
  },
};
</script>

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

h1,
h2,
h3 {
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

.section {
  padding-block: 5rem 2rem;
}

.section__title {
  text-align: center;
  font-size: var(--h1-font-size);
  font-weight: var(--font-bold);
  margin-bottom: 2rem;
}

.main {
  overflow: hidden;
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

.nav__toggle,
.nav__close {
  font-size: 1.5rem;
  color: var(--title-color);
  cursor: pointer;
}

@media screen and (max-width: 1150px) {
  .nav__menu {
    position: fixed;
    top: 0;
    right: -100%;
    background-color: hsla(var(--hue), 70%, 4%, .2);
    backdrop-filter: blur(16px);
    -webkit-backdrop-filter: blur(16px);
    width: 80%;
    height: 100%;
    padding: 7rem 3rem;
    transition: right .4s;
  }
}

.nav__list {
  display: flex;
  flex-direction: column;
  row-gap: 3rem;
}

.nav__link {
  position: relative;
  color: var(--title-color);
  font-weight: var(--font-semi-bold);
  transition: color .4s;
}

.nav__link::after {
  content: '';
  width: 0;
  height: 2px;
  background-color: var(--first-color-light);
  position: absolute;
  left: 0;
  bottom: -.5rem;
  transition: width .3s;
}

.nav__link:hover {
  color: var(--first-color-light);
}

.nav__link:hover::after {
  width: 30%;
}

.nav__close {
  position: absolute;
  top: 1rem;
  right: 1.5rem
}

.show-menu {
  right: 0;
}

/* Home */
.home__container {
  row-gap: 2rem;
  padding-top: 1rem;
}

.home__img {
  width: 220px;
  justify-self: center;
  mask-image: linear-gradient(to bottom, hsla(var(--hue), 40%, 16%) 60%, transparent 100%);
}

.home__name {
  font-size: var(--biggest-font-size);
  font-weight: var(--font-bold);
  word-break: break-word;
  margin-bottom: 1rem;
}

.home__profession {
  position: relative;
  font-size: var(--big-font-size);
  color: var(--text-color);
}

.home__profession::after {
  content: '';
  position: absolute;
  width: 25%;
  height: 3px;
  background-color: var(--text-color);
  left: 0;
  bottom: -.5rem;
}

.home__scroll {
  color: var(--title-color);
  display: inline-flex;
  
}

</style>
