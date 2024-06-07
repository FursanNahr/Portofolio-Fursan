<template>
  <div id="app">
    <nav>
      <div>
        <div class="logo"><img class="logo foto-logo" src="../assets/images/image-removebg-preview.png" alt=""></div>
      </div>
      <div>
        <div class="text-li">
          <div class="a">
            <RouterLink class="a-nav" to="/">Home</RouterLink>
            <div class="hover-nav"></div>
          </div>
          <div class="a">
            <RouterLink class="a-nav" to="/">Work</RouterLink>
            <div class="hover-nav"></div>
          </div>
          <div class="a">
            <RouterLink class="a-nav" to="/">My Info</RouterLink>
            <div class="hover-nav"></div>
          </div>
          <div class="a">
            <RouterLink class="a-nav" to="/">Service</RouterLink>
            <div class="hover-nav"></div>
          </div>
          <div class="a">
            <RouterLink class="a-nav" to="/">Contact Me</RouterLink>
            <div class="hover-nav"></div>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&display=swap');

body {
  background-color: #101010;
  color: white;
  font-family: "Poppins";
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

.a-nav {
  color: white;
  text-decoration: none;
}
.a-nav:hover {
  color: #ff6205;
  transition: color 1s;
}
.a:hover .hover-nav {
  width: 2vw;
  height: 0.15vw;
  background-color: #ff6205; 
}
.logo {
  margin: 0 auto;
  height: 4vw;
  width: fit-content;
}
</style>
