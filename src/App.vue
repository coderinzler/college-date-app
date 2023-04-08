<script setup>
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
import HeaderImage from "./components/HeaderImage.vue";
import TopBar from "@/components/TopBar.vue";
</script>

<template>
  <Header class="header"></Header>
  <main>
  <HeaderImage />
  <TopBar class="topbar" />
  <Footer class="footer" />
  </main>
</template>

<style scoped>

main{
    grid-column: span 2;
    display: grid;
    margin-top: 100px;
    grid-template-columns: 1fr 3fr;
    grid-template-rows: 1fr 10fr 1fr;
}
.header{
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 100;
}

.topbar{
  grid-column: span 3;
  bottom: 44px;
}
.footer {
    background-color: red;
    grid-column: span 3;
}

</style>
