<script setup>
  import Header from "./components/Header.vue"
  import HeroSection from "./components/HeroSection.vue"
</script>

<template>
  <div class="page">
    <Header class="header--absolute" />
    <HeroSection />
  </div>
</template>

<style scoped>
/* .header--absolute {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 10;
  background: transparent;
} */
</style>
