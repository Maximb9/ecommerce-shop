<script setup>
import Header from "./components/Layout/Header.vue";
import Hero from "./components/Hero.vue";
</script>

<template>
  <div class="container">
    <Header />
    <Hero />
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style lang="scss">
@import url('https://fonts.cdnfonts.com/css/satoshi');
@import url('https://fonts.cdnfonts.com/css/clash-display');

*{
  box-sizing: border-box;
}

body {
  font-family: 'Satoshi', sans-serif;
  margin: 0;
  padding: 0;
  font-size: 16px;
  //font-family: 'Clash Display', sans-serif;
}

img {
  max-width: 100%;
}

.container {
  max-width: 1440px;
  margin: auto;
}
</style>
