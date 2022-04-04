<template>
  <nav-bar></nav-bar>
  <the-hero></the-hero>
  <main-content></main-content>
  <the-gallery></the-gallery>
  <the-footer></the-footer>
</template>

<script>
import TheHero from "./components/TheHero.vue";
import NavBar from "./components/NavBar.vue";
import MainContent from "./components/MainContent.vue";
import TheGallery from "./components/TheGallery.vue";
import TheFooter from "./components/TheFooter.vue";
export default {
  components: { TheHero, NavBar, MainContent, TheGallery, TheFooter },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Alata&family=Josefin+Sans:wght@300&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  scroll-behavior: smooth;
}
h1,
h2,
ul {
  font-family: "Josefin Sans", sans-serif;
  text-transform: uppercase;
}
h2 {
  font-size: 2rem;
}

p {
  font-family: "Alata", sans-serif;
  color: hsl(0, 0%, 55%);
  font-size: 15px;
}
a {
  text-decoration: none;
  color: inherit;
}
ul {
  list-style: none;
}
</style>
