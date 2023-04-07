<script setup>
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
</script>

<template>
  <main>
    <Header/>
    <div class="side"></div>
    <div class="center"></div>
    <Footer class="footer" />
  </main>
</template>

<style scoped>
main {
  grid-column: span 2;
  display: grid;
  grid-template-columns: 1fr 3fr;
  grid-template-rows: 2fr 10fr 1fr;
}
.footer {
  background-color: red;
  grid-column: span 3;
}
.center {
  grid-column: span 2;
  display: grid;
  grid-template-rows: 1fr 1fr;
  grid-template-columns: 1fr 1fr;
  background-color: yellow;
  grid-gap: 60px 120px;
  padding: 40px;
}
.side {
  grid-column: span 1;
  background-color: blue;
  display: grid;
  grid-template-rows: 1fr 1fr 1fr;
  grid-gap: 20px;
  padding: 20px;
}
</style>
