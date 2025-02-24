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
            <a href="#home" class="nav__link">Beranda</a>
          </li>
          <li>
            <a href="#work" class="nav__link">Pekerjaan</a>
          </li>
          <li>
            <a href="#info" class="nav__link">Informasi</a>
          </li>
          <li>
            <a href="#service" class="nav__link">Layanan</a>
          </li>
          <li>
            <a href="#contact" class="nav__link">Kontak</a>
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
          <h3 class="home__profession">Front-End Developer</h3>
        </div>

        <a href="#work" class="home__scroll">
          <div class="home__scroll-box">
            <i class="ri-arrow-down-line"></i>
          </div>

          <span class="home__scroll-text">Pekerjaan Terbaru</span>
        </a>
      </div>
    </section>

    <section class="work section" id="work">
      <h2 class="section__title">
        PEKERJAAN TERBARU
      </h2>
      <div class="work__container container grid">
        <article class="work__card">
          <a href="https://ajibtest.online/" target="_blank" class="work__link">
            <h2 class="work__title">Website Absensi SMK 4</h2>
            <p class="work__description">
              29/2/24 <br> menjadi Front-end untuk website Absensi SMK 4
            </p>

            <img src="../assets/images/work1.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>

        <article class="work__card">
          <a href="#" target="_blank" class="work__link">
            <h2 class="work__title">Website Keraton</h2>
            <p class="work__description">
              29/2/24 <br> menjadi front-end untuk website Keraton
            </p>

            <img src="../assets/images/work2.png" class="work__img" alt="">

            <i class="ri-arrow-right-line"></i>
          </a>
        </article>
      </div>
    </section>
    <section class="info section" id="info">
      <h2 class="section__title">TENTANG SAYA</h2>

      <div class="info__container container grid">
        <!-- TENTANG -->
        <div class="about grid">
          <div class="about__content">
            <h3 class="info__title">Tentang Saya</h3>
            <p class="about__description">
              Bersemangat dalam Membuat Website. Saya memiliki pengalaman beberapa tahun sebagai
              <b>front-end developer</b> dengan beberapa proyek yang telah diselesaikan.
            </p>

            <button @click="downloadCV" class="button about__button">Unduh CV</button>
          </div>

          <img src="../assets/images/fotoukur.png" alt="" class="about__img">
        </div>

        <!-- Experience -->
        <div class="experience">
          <h3 class="info__title">Pengalaman</h3>

          <div class="experience__content grid">
            <div class="experience__data grid">
              <h2 class="experience__company grid">PT. Curaweda</h2>

              <div>
                <h3 class="experience__profession">Web Front-End</h3>
                <span class="experience__date">02/24 - 06/24</span>
                <p class="experience__description">
                  Menjadi front-end dalam pembuatan website Absensi SMK 4 dan Keraton
                </p>
              </div>
            </div>
          </div>
        </div>


        <div class="skills">
          <h3 class="info__title">Keahlian</h3>

          <div class="skills">
            <h3 class="info__title">Keahlian</h3>
            <!-- Highlight Box -->
            <div id="highlightBox" class="highlight">
              <p id="highlightText">Klik ikon untuk melihat detail keahlian</p>
            </div>
            <div class="skills__content grid">
              <div class="skills__box"
                data-skill="HTML (Mahir) - Menguasai pembuatan struktur halaman web yang rapi, efisien, dan sesuai standar dengan elemen semantik.">
                <img src="../assets/images/HTML-5-Badge-Logo.png" alt="" class="skills__img">
                <span class="skills__name">HTML</span>
              </div>

              <div class="skills__box"
                data-skill="CSS (Mahir) - Menguasai styling halaman web dengan CSS modern, mencakup desain responsif, animasi, fleksibilitas layout, serta optimasi untuk berbagai perangkat dan browser.">
                <img src="../assets/images/css.png" alt="" class="skills__img">
                <span class="skills__name">CSS</span>
              </div>

              <div class="skills__box"
                data-skill="Vue js (Ahli) - Menguasai framework Vue.js dengan keahlian tingkat tinggi, mampu merancang dan mengembangkan aplikasi web yang kompleks dan scalable, mengoptimalkan state management, serta menerapkan best practices dalam setiap aspek pengembangan front-end.">
                <img src="../assets/images/Vue.png" alt="" class="skills__img">
                <span class="skills__name">Vue JS</span>
              </div>

              <div class="skills__box"
                data-skill="React (Ahli) - Menguasai secara mendalam pengembangan aplikasi web dengan React, mampu merancang arsitektur komponen yang kompleks, mengoptimalkan performa melalui advanced hooks dan teknik state management, serta menerapkan best practices untuk membangun UI interaktif dan scalable">
                <img src="../assets/images/react.png" alt="" class="skills__img">
                <span class="skills__name">React</span>
              </div>
              <div class="skills__box"
                data-skill="JavaScript (Mahir) - Menguasai bahasa pemrograman JavaScript secara menyeluruh, mampu menerapkan konsep-konsep ES6+, asynchronous programming, dan manipulasi DOM untuk membangun aplikasi web interaktif dan dinamis.">
                <img src="../assets/images/javascript.png" alt="" class="skills__img">
                <span class="skills__name">JavaScript</span>
              </div>
              <div class="skills__box"
                data-skill="TypeScript (Menengah) - Mampu menggunakan TypeScript untuk menambah kejelasan dan keamanan kode, serta mengintegrasikannya dalam proyek pengembangan aplikasi web dengan pemahaman yang baik tentang konsep-konsep dasar dan lanjutan.">
                <img src="../assets/images/typescript.png" alt="" class="skills__img">
                <span class="skills__name">TypeScript</span>
              </div>

              <div class="skills__box"
                data-skill="GitHub (Mahir) - Menguasai penggunaan GitHub untuk kolaborasi, version control, dan integrasi dengan workflow pengembangan modern, serta familiar dengan berbagai fitur seperti pull request, issue tracking, dan GitHub Actions.">
                <img src="../assets/images/github.png" alt="" class="skills__img">
                <span class="skills__name">GitHub</span>
              </div>

              <div class="skills__box"
                data-skill="Tailwind (Ahli) - Menguasai penggunaan Tailwind CSS secara mendalam, mampu membangun antarmuka yang responsif dan estetis dengan utility-first approach, serta mengoptimalkan workflow styling melalui custom configuration dan integrasi yang efisien dalam proyek pengembangan modern.">
                <img src="../assets/images/tailwind.png" alt="" class="skills__img">
                <span class="skills__name">Tailwind</span>
              </div>
              <div class="skills__box"
                data-skill="SCSS (Mahir) - Menguasai penulisan gaya dengan SCSS, termasuk penggunaan variabel, nested rules, mixins, inheritance, dan optimasi kode untuk meningkatkan efisiensi serta maintainability.">
                <img src="../assets/images/scss.png" alt="" class="skills__img">
                <span class="skills__name">SCSS</span>
              </div>

              <div class="skills__box"
                data-skill="Bootstrap (Menengah) - Mampu membangun tampilan responsif dengan komponen dan grid system Bootstrap, serta menyesuaikan styling menggunakan custom CSS atau SCSS.">
                <img src="../assets/images/Bootstrap.png" alt="" class="skills__img">
                <span class="skills__name">Bootstrap</span>
              </div>


            </div>
          </div>

        </div>
      </div>
    </section>

    <section class="services section" id="service">
      <h2 class="section__title">LAYANAN</h2>

      <div class="services__container container grid">

        <article class="services__card">
          <i class="ri-code-box-line services__icon"></i>

          <h3 class="services__title">Front-End</h3>
          <p class="services__description">
            Layanan front-end kami dirancang untuk membangun antarmuka pengguna yang intuitif dan interaktif,
            memastikan proyek Anda terlihat profesional dan berfungsi dengan baik.
          </p>
        </article>

        <article class="services__card">
          <i class="ri-layout-2-line services__icon"></i>

          <h3 class="services__title">Web Responsif</h3>
          <p class="services__description">
            Kami menawarkan pengembangan web responsif untuk memastikan situs Anda tampil sempurna di semua perangkat.
          </p>
        </article>
      </div>
    </section>

    <section class="contact section" id="contact">
      <h2 class="section__title">HUBUNGI SAYA</h2>

      <div class="contact__container container grid">
        <form action="" class="contact__form grid" id="contact-form">
          <div class="contact__group grid">
            <input type="text" placeholder="Nama" required class="contact__input" name="" id="">
            <input type="email" placeholder="Email" required class="contact__input" name="" id="">
          </div>

          <textarea name="" placeholder="Pesan" required class="contact__input contact__area" id=""></textarea>

          <button type="submit" class="button contact__button">Kirim Pesan</button>

          <p class="contact__message" id="contact-message"></p>
        </form>

        <div class="contact__social grid">
          <a href="https://www.instagram.com/fursannr_/" target="_blank" class="contact__social-link">
            <i class="ri-instagram-line"></i>
            <span>Instagram</span>
          </a>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="footer__container container grid">
      <ul class="footer__links">
        <li>
          <a href="#home" class="footer__link">Beranda</a>
        </li>
        <li>
          <a href="#work" class="footer__link">Pekerjaan</a>
        </li>
        <li>
          <a href="#info" class="footer__link">Info</a>
        </li>
      </ul>

      <span class="footer__copy">
        &#169; Seluruh Hak Cipta Dilindungi oleh Ukur
      </span>
    </div>
  </footer>

  <!-- Scroll Up -->
  <a href="#" :class="{ 'show-scroll': isShowScroll }" class="scrollup" id="scroll-up">
    <i class="ri-arrow-up-line"></i>
  </a>
</template>
<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue';

const isBlurred = ref(false);
const isShowScroll = ref(false);

const downloadCV = () => {
  // Path ke file PDF
  const fileUrl = '../assets/text/cvFursan.pdf';
  
  fetch(fileUrl)
    .then(response => {
      if (!response.ok) {
        throw new Error('Network response was not ok');
      }
      return response.blob();
    })
    .then(blob => {
      // Buat URL object untuk blob
      const url = window.URL.createObjectURL(blob);
      
      // Buat elemen <a> secara programatis
      const link = document.createElement('a');
      link.href = url;
      link.setAttribute('download', 'cvFursan.pdf');
      
      // Append ke body, klik, lalu hapus
      document.body.appendChild(link);
      link.click();
      
      // Clean up
      window.URL.revokeObjectURL(url);
      document.body.removeChild(link);
    })
    .catch(error => {
      console.error('Error downloading file:', error);
      alert('Gagal mengunduh file. Silakan coba lagi nanti.');
    });
};

document.addEventListener("DOMContentLoaded", function () {
  const skillBoxes = document.querySelectorAll(".skills__box");
  const highlightBox = document.getElementById("highlightBox");
  const highlightText = document.getElementById("highlightText");

  skillBoxes.forEach(box => {
    box.addEventListener("click", function () {
      const skillInfo = this.getAttribute("data-skill");
      highlightText.textContent = skillInfo;
      highlightBox.style.display = "block";
    });
  });
});


// Methods
const blurHeader = () => {
  isBlurred.value = window.scrollY >= 50;
  isShowScroll.value = window.scrollY >= 350;
};

const scrollActive = () => {
  const sections = document.querySelectorAll('section[id]');
  const scrollDown = window.scrollY;
  console.log('scrollActive called'); // Debugging: log ketika scrollActive dipanggil

  sections.forEach(current => {
    const sectionHeight = current.offsetHeight,
      sectionTop = current.offsetTop - 58,
      sectionId = current.getAttribute('id'),
      sectionsClass = document.querySelector('.nav__menu a[href*=' + sectionId + ']');
    console.log(`Checking section: ${sectionId}`); // Debugging: log setiap section

    if (scrollDown > sectionTop && scrollDown <= sectionTop + sectionHeight) {
      console.log(`Adding active-link to: ${sectionId}`); // Debugging: log ketika menambahkan kelas
      sectionsClass.classList.add('active-link');
    } else {
      console.log(`Removing active-link from: ${sectionId}`); // Debugging: log ketika menghapus kelas
      sectionsClass.classList.remove('active-link');
    }
  });
};

// Lifecycle hooks
onMounted(() => {
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

  // Add Blur Header and Scroll Active listeners
  window.addEventListener('scroll', blurHeader);
  window.addEventListener('scroll', scrollActive);
});

onBeforeUnmount(() => {
  window.removeEventListener('scroll', blurHeader);
  window.removeEventListener('scroll', scrollActive);
});
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

/* Active Link */
.active-link {
  color: var(--first-color-light);
}

.active-link::after {
  width: 30%;
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

.work__img {
  width: 444px;
  height: 250px;
  object-fit: cover
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

/* Highlight Box */
.highlight {
  margin-top: 1rem;
  padding: 1rem;
  background: #f4f4f4;
  border-left: 5px solid #007bff;
  font-weight: bold;
  color: var(--container-color);
  ;
  display: none;
  margin-bottom: 10px;
  /* Sembunyikan awalnya */
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

/* Contact */
.contact__container {
  row-gap: 4rem;
}

.contact__group,
.contact__form {
  gap: 1rem;
}

.contact__form {
  position: relative;
}

.contact__input {
  padding: 1.25rem;
  background-color: var(--container-color);
  color: var(--title-color);
}

.contact__input::placeholder {
  color: var(--text-color-light);
}

.contact__area {
  height: 10rem;
  resize: none
}

.contact__button {
  margin-top: 1rem;
  cursor: pointer;
}

.contact__social {
  grid-template-columns: repeat(1, max-content);
  justify-content: center;
  column-gap: 3rem;
}

.contact__social-link {
  color: var(--title-color);
  display: inline-flex;
  column-gap: .25rem;
  align-items: center;
  transition: color .4s;
}

.contact__social-link i {
  font-size: 1.5rem;
}

.contact__social-link span {
  font-size: var(--small-font-size);
  font-weight: var(--font-semi-bold);
}

.contact__social-link:hover {
  color: var(--first-color-light);
}

.contact__message {
  position: absolute;
  left: 0;
  bottom: -2rem;
  font-size: var(--small-font-size);
  font-weight: var(--font-semi-bold);
  color: var(--title-color);
}

/* Footer */
.footer {
  background-color: var(--container-color);
}

.footer__container {
  padding-block: 3rem 2rem;
  row-gap: 3rem;
}

.footer__links {
  display: flex;
  justify-content: center;
  column-gap: 2.5rem;
}

.footer__link {
  color: var(--title-color);
  font-weight: var(--font-semi-bold);
  transition: color .4s;
}

.footer__link:hover {
  color: var(--first-color-light);
}

.footer__copy {
  color: var(--title-color);
  font-size: var(--small-font-size);
  text-align: center;
}

/* Scroll Bar */
::-webkit-scrollbar {
  width: 0.6rem;
  background-color: hsl(var(--hue), 20%, 20%);
}

::-webkit-scrollbar-thumb {
  background-color: hsl(var(--hue), 20%, 30%);
}

::-webkit-scrollbar-thumb:hover {
  background-color: hsl(var(--hue), 20%, 40%);
}

/* Scrorll Up */
.scrollup {
  position: fixed;
  right: 1rem;
  bottom: -50%;
  background-color: var(--container-color);
  display: inline-flex;
  padding: 6px;
  color: var(--title-color);
  font-size: 1.25rem;
  box-shadow: 0 4px 12px hsla(var(--hue), 30% 8% .3);
  z-index: var(--z-tooltip);
  transition: bottom .4s, transform .4s;
}

.scrollup:hover {
  transform: translateY(-.5rem);
}

/* Show scroll up */
.show-scroll {
  bottom: 3rem;
}

/* Breakpoints */
/* For small device */
@media screen and (max-width: 300px) {
  .container {
    margin-inline: 1rem;
  }

  .skills__content {
    grid-template-columns: repeat(2, max-content);
  }
}

/* For medium device */
@media screen and (min-width: 540px) {

  .home__container,
  .work__container,
  .info__container,
  .services__container,
  .contact__container {
    grid-template-columns: 350px;
    justify-content: center;
  }
}

@media screen and (min-width: 768px) {
  .nav__menu {
    width: 50%;
  }

  .home__container {
    grid-template-columns: repeat(2, 350px);
  }

  .home__data {
    align-self: flex-end;
    padding-bottom: 3rem;
    order: -1;
  }

  .home__scroll {
    grid-column: 1 / 3;
  }

  .work__container {
    grid-template-columns: repeat(2, 350px)
  }

  .info__container {
    grid-template-columns: initial;
  }

  .about {
    grid-template-columns: repeat(2, 350px);
    align-items: center;
  }

  .about__content {
    order: 1;
  }

  .experience__data {
    grid-template-columns: repeat(2, 1fr);
  }

  .skills__content {
    grid-template-columns: repeat(5, max-content);
    justify-content: initial;
    column-gap: 4rem;
  }

  .services__container {
    grid-template-columns: repeat(2, 328px);
  }
}

/* For Large Device */
@media screen and (min-width: 1150px) {
  .container {
    margin-inline: auto;
  }

  .section {
    padding-block: 7rem 5rem;
  }

  .section__title {
    margin-bottom: 4rem;
  }

  .nav {
    height: calc(var(--header-height) + 2rem);
  }

  .nav__close,
  .nav__toggle {
    display: none;
  }

  .nav__menu {
    width: initial;
  }

  .nav__list {
    flex-direction: row;
    column-gap: 4rem;
  }

  .home__container {
    grid-template-columns: 375px 350px;
    gap: 3rem 16rem;
  }

  .home__img {
    width: 350px;
  }

  .home__name {
    margin-bottom: 1.5rem
  }

  .home__profession::after {
    bottom: -1rem;
    width: 35%;
  }

  .work__container {
    grid-template-columns: repeat(2, 540px);
    gap: 2.5rem;
  }

  .work__link {
    padding: 3rem 3rem 2rem;
  }

  .work__title {
    font-size: var(--h2-font-size);
    margin-bottom: 1rem;
  }

  .work__link i {
    font-size: 2rem;
  }

  .info__container {
    row-gap: 4rem;
  }

  .info__title {
    font-size: var(--normal-font-size);
    margin-bottom: 3.5rem;
  }

  .about {
    grid-template-columns: 320px 420px;
  }

  .about__img {
    width: 320px;
  }

  .about__description {
    margin-bottom: 3rem;
  }

  .about__button {
    width: initial;
  }

  .experience__content {
    row-gap: 4rem;
  }

  .experience__data {
    grid-template-columns: 320px 380px;
    column-gap: 11.5rem;
  }

  .experience__company {
    font-size: var(--h1-font-size);
  }

  .experience__profession {
    margin-bottom: .5rem;
  }

  .experience__date {
    font-size: var(--normal-font-size);
  }

  .skills__content {
    grid-template-columns: repeat(6, max-content);
  }

  .services__container {
    grid-template-columns: repeat(2, 350px);
    gap: 6rem 13rem;
  }

  .services__icon {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
  }

  .contact__container {
    grid-template-columns: 580px;
  }

  .contact__group {
    grid-template-columns: repeat(2, 1fr);
  }

  .contact__area {
    height: 15rem;
  }

  .contact__button {
    width: max-content;
    justify-self: center;
    margin-top: 1.5rem;
  }

  .contact__message {
    bottom: 4.5rem
  }

  .footer__container {
    padding-block: 3rem;
    grid-template-columns: repeat(2, max-content);
    justify-content: space-between;
  }

  .footer__links {
    column-gap: 4rem;
    order: 1;
  }

  .scrollup {
    right: 3rem;
  }
}
</style>
