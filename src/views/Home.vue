<template>
  <!-- RemixIcon -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/remixicon/4.2.0/remixicon.min.css"
    integrity="sha512-MqL4+Io386IOPMKKyplKII0pVW5e+kb+PI/I3N87G3fHIfrgNNsRpzIXEi+0MQC0sR9xZNqZqCYVcC61fL5+Vg=="
    crossorigin="anonymous" referrerpolicy="no-referrer" />

  <!-- HEADER -->
  <header :class="{ 'blur-header': isBlurred }" class="header" id="header">
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
      <h2 class="section__title">
        RECENT WORK
      </h2>
      <div class="work__container container grid">
        <article class="work__card">
          <a href="#" target="_blank" class="work__link">
            <h2 class="work__title">Restaurant Website</h2>
            <p class="work__description">
              Short description of the project that was carried out in this portofolio.
            </p>

            <img src="../assets/images/work1.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>

        <article class="work__card">
          <a href="#" target="_blank" class="work__link">
            <h2 class="work__title">Restaurant Website</h2>
            <p class="work__description">
              Short description of the project that was carried out in this portofolio.
            </p>

            <img src="../assets/images/work1.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>

        <article class="work__card">
          <a href="#" target="_blank" class="work__link">
            <h2 class="work__title">Restaurant Website</h2>
            <p class="work__description">
              Short description of the project that was carried out in this portofolio.
            </p>

            <img src="../assets/images/work1.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>

        <article class="work__card">
          <a href="#" target="_blank" class="work__link">
            <h2 class="work__title">Restaurant Website</h2>
            <p class="work__description">
              Short description of the project that was carried out in this portofolio.
            </p>

            <img src="../assets/images/work1.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>

        <article class="work__card">
          <a href="#" target="_blank" class="work__link">
            <h2 class="work__title">Restaurant Website</h2>
            <p class="work__description">
              Short description of the project that was carried out in this portofolio.
            </p>

            <img src="../assets/images/work1.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>
      </div>
    </section>
    <section class="info section" id="info">
      <h2 class="section__title">MY INFO</h2>

      <div class="info__container container grid">
        <!-- ABOUT -->
        <div class="about grid">
          <div class="about__content">
            <h3 class="info__title">About Me</h3>
            <p class="about__description">
              Passionate About Creating <b>Websites with beautiful interface</b>. I have years of experience in <b>Web
                Development</b> with several projects completed.
            </p>

            <a href="../assets/text/CV_Fursan Nahr.pdf" download="" target="_blank"
              class="button about__button">Download CV</a>
          </div>

          <img src="../assets/images/fotoukur.png" alt="" class="about__img">
        </div>

        <!-- Experience -->
        <div class="experience">
          <h3 class="info__title">Experience</h3>

          <div class="experience__content grid">
            <div class="experience__data grid">
              <h2 class="experience__company grid">Discord</h2>

              <div>
                <h3 class="experience__profession">Web Product Designer</h3>
                <span class="experience__date">05/23 - Present</span>
                <p class="experience__description">
                  Short description of the work you do or did in the company
                </p>
              </div>
            </div>

            <div class="experience__data grid">
              <h2 class="experience__company grid">Google</h2>

              <div>
                <h3 class="experience__profession">Web Developer</h3>
                <span class="experience__date">05/23 - Present</span>
                <p class="experience__description">
                  Short description of the work you do or did in the company
                </p>
              </div>
            </div>

            <div class="experience__data grid">
              <h2 class="experience__company grid">Adobe</h2>

              <div>
                <h3 class="experience__profession">Web Designer</h3>
                <span class="experience__date">05/23 - Present</span>
                <p class="experience__description">
                  Short description of the work you do or did in the company
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="skills">
          <h3 class="info__title">Skills</h3>

          <div class="skills__content grid">

            <div class="skills__box">
              <img src="../assets/images/HTML-5-Badge-Logo.png" alt="" class="skills__img">
              <span class="skills__name">HTML</span>
            </div>

            <div class="skills__box">
              <img src="../assets/images/css.png" alt="" class="skills__img">
              <span class="skills__name">CSS</span>
            </div>
            <div class="skills__box">
              <img src="../assets/images/scss.png" alt="" class="skills__img">
              <span class="skills__name">SCSS</span>
            </div>

            <div class="skills__box">
              <img src="../assets/images/bootstrap.png" alt="" class="skills__img">
              <span class="skills__name">Bootstrap</span>
            </div>

            <div class="skills__box">
              <img src="../assets/images/vue.png" alt="" class="skills__img">
              <span class="skills__name">Vue JS</span>
            </div>

            <div class="skills__box">
              <img src="../assets/images/github.png" alt="" class="skills__img">
              <span class="skills__name">Github</span>
            </div>

          </div>
        </div>
      </div>
    </section>

    <section class="services section" id="services">
      <h2 class="section__title">SERVICE</h2>

      <div class="services__container container grid">

        <article class="services__card">
          <i class="ri-code-box-line services__icon"></i>

          <h3 class="services__title">Web Development</h3>
          <p class="services__description">
            Short description of the service offered to users
            to obtain a personalized project.
          </p>
        </article>

        <article class="services__card">
          <i class="ri-layout-2-line services__icon"></i>

          <h3 class="services__title">Responsive Web Design</h3>
          <p class="services__description">
            Short description of the service offered to users
            to obtain a personalized project.
          </p>
        </article>

        <article class="services__card">
          <i class="ri-seo-line services__icon"></i>

          <h3 class="services__title">Seo (Web Pages)</h3>
          <p class="services__description">
            Short description of the service offered to users
            to obtain a personalized project.
          </p>
        </article>
        
      </div>
    </section>

    <section class="contact section" id="contact">
      <h2 class="section__title">CONTACT ME</h2>

      <div class="contact__container container grid">
        <form action="" class="contact__form grid" id="contact-form">
          <div class="contact__group grid">
            <input type="text" placeholder="Names" required class="contact__input" name="" id="">
            <input type="email" placeholder="Email" required class="contact__input" name="" id="">
          </div>

          <textarea name="" placeholder="Message" required class="contact__input contact__area" id=""></textarea>

          <button type="submit" class="button contact__button">Send Messages</button>

          <p class="contact__message" id="contact-message"></p>
        </form>

        
      </div>
    </section>
  </main>
</template>
<script>
export default {
  data() {
    return {
      isBlurred: false,
    };
  },
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

    // Add Blur Header
    window.addEventListener('scroll', this.blurHeader);
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.blurHeader);
  },
  methods: {
    blurHeader() {
      this.isBlurred = window.scrollY >= 50;
    },
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

/* Blur Header */
.blur-header::after {
  content: '';
  position: absolute;
  width: 1000%;
  height: 100%;
  background-color: hsla(var(--hue), 70%, 4%, .2);
  backdrop-filter: blur(16px);
  -webkit-backdrop-filter: blur(16px);
  top: 0;
  left: 0;
  z-index: -1;
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
  column-gap: .5rem;
  align-items: center;
  justify-self: center;
  margin-top: 3rem;
}

.home__scroll-box {
  background-color: var(--first-color);
  width: 32px;
  height: 32px;
  display: grid;
  place-items: center;
  font-size: 1.5rem;
  overflow: hidden;
}

.home__scroll-text {
  font-weight: var(--font-semi-bold);
}

.home__scroll-box i {
  animation: scroll-down 3s infinite;
}

@keyframes scroll-down {
  0% {
    transform: translateY(-1rem);
    opacity: 0;
  }

  50% {
    transform: translateY(0);
    opacity: 1;
  }

  100% {
    transform: translateY(1rem);
    opacity: 0;
  }
}

/* Scroll */
.work {
  background-color: var(--container-color);
}

.work__card {
  background-color: var(--first-color);
}

.work__link {
  display: block;
  position: relative;
  background-color: var(--body-color);
  padding: 2rem 1.5rem 1.5rem 1.5rem;
  color: var(--text-color);
  transition: transform .4s;
}

.work__title {
  font-size: var(--h3-font-size);
  margin-bottom: .75rem;
}

.work__description {
  margin-bottom: 1.5rem;
}

.work__link i {
  position: absolute;
  top: 1.8rem;
  right: 1.5em;
  font-size: 1.5rem;
  color: var(--first-color);
  transition: transform .4s;
}

.work__link:hover {
  transform: translateY(-.35rem);
}

.work__link:hover i {
  transform: translateX(.5rem);
}

/* INFO */

.info__container {
  row-gap: 3rem;
}

.info__title {
  position: relative;
  font-size: var(--small-font-size);
  color: var(--text-color);
  margin-bottom: 2rem;
}

.info__title::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: -.5rem;
  width: 20px;
  height: 2px;
  background-color: var(--text-color);
}

/* ABOUT */
.about {
  row-gap: 3rem;
}


.about__description {
  margin-bottom: 2rem;
}

.about__description b {
  color: var(--first-color-light);
}

.about__button {
  width: 100%;
}

.about__img {
  width: 250px;
  justify-self: center;
  mask-image: linear-gradient(to bottom, hsla(var(--hue), 40%, 16%) 60%, transparent 100%);
}

/* BUTTON */
.button {
  display: inline-flex;
  justify-content: center;
  background-color: var(--first-color);
  color: var(--title-color);
  font-weight: var(--font-semi-bold);
  padding: 1.25rem 2rem;
  transition: background-color .4s;
}

.button:hover {
  background-color: var(--first-color-alt);
}
/* Experience */
.experience__content {
  row-gap: 2rem;
}

.experience__data {
  row-gap: 1rem;
}

.experience__company {
  font-size: var(--h2-font-size);
  font-weight: var(--font-bold);
}

.experience__profession {
  font-size: var(--h3-font-size);
  margin-bottom: .25rem;
}

.experience__date {
  display: block;
  font-size: var(--small-font-size);
  margin-bottom: .75rem;
}

/* Skills */
.skills__img {
  width: 35px;
}

.skills__name {
  font-size: var(--small-font-size);
}

.skills__content {
  grid-template-columns: repeat(3, max-content);
  justify-content: space-around;
  align-items: flex-end;
}

.skills__box {
  display: grid;
  place-items: center;
  transition: transform .4s;
}

.skills__box:hover {
  transform: translateY(-.25rem);
}

/* Services */
.services {
  background-color: var(--container-color);
}
.services__container {
  row-gap: 2rem;
}
.services__icon {
  display: block;
  color: var(--first-color-light);
  font-size: 2rem;
  margin-bottom: 2rem;
}
.services__title {
  font-size: var(--h3-font-size);
  margin-bottom: 0.75rem
}
</style>
