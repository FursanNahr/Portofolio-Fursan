<template>
  <div id="app">
    <nav>
      <div>
        <div class="logo"><img class="logo foto-logo" src="../assets/images/image-removebg-preview.png" alt=""></div>
      </div>
      <div>
        <div class="text-li">
          <div class="a">
            <a href="#home" class="hover-line">Home</a>
          </div>
          <div class="a">
            <a href="#work" class="hover-line">Work</a>
          </div>
          <div class="a">
            <a href="#info" class="hover-line">My Info</a>
          </div>
          <div class="a">
            <a href="#service" class="hover-line">Service</a>
          </div>
          <div class="a">
            <a href="#contact" class="hover-line">Contact</a>
          </div>
        </div>
      </div>
    </nav>

    <div class="container-foto-nama">
      <div>
        <div>Fursan Nahr</div>
        <div>Front-End Developer</div>
      </div>
      <div>
        <img src="../assets/images/fotoukur.png" alt="">
      </div>
    </div>
  </div>
</template>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400..800&display=swap');

body {
  background-color: #101010;
  color: white;
  font-family: "Syne";
}

nav {
  display: flex;
  align-items: center;
  width: 100%;
  height: 4vw;
}

.text-li {
  display: flex;
  width: 90%;
}

nav div:nth-child(1) {
  flex: 1;
  color: #eb6e26;
}

nav>div:nth-child(2) {
  flex: 1.5;
}

.a {
  flex: 1;
  width: 1vw;
}

.logo {
  margin: 0 auto;
  height: 4vw;
  width: fit-content;
}



.hover-line {
  position: relative;
  padding-bottom: 0.4vw;
  color: white;
  font-size: 1.2vw;
  text-decoration: none;
}

.hover-line::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: 0;
  width: 0;
  height: 0.15vw;
  background-color: #f95b04;
  transition: width 0.3s ease-out;
}

.hover-line:hover {
  color: #f95b04;
  transition: 0.3s ease-out;
}

.hover-line:hover::after {
  width: 30%;
}
.container-foto-nama {
  display: flex;
  margin: 10vw auto 0 auto;
  width: fit-content;
  align-items: center;
}
.container-foto-nama img{
  height: 30vw;
}
.container-foto-nama div div:first-child {
  font-size: 5vw;
  font-weight: 700;
  width: 50%;
  line-height: 5vw;
  color: #ff5f00;
}
.container-foto-nama div div:last-child {
  font-size: 3vw;
  font-weight: 600;
}
.container-foto-nama div:first-child {
  padding-right: 5vw;
}
</style>
