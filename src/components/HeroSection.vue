<script setup>
  import HeroContent from './HeroContent.vue';
</script>

<template>
  <section class="hero">
    <HeroContent />
  </section>
</template>

<style scoped>
.hero {
  background-color: hsl(257, 40%, 49%);
  background-image: url("@/assets/images/bg-mobile.svg");
  background-repeat: no-repeat;
  background-position: center top;
  background-size: 100vw;
  padding-top: 130px;
  /* background-position: center; */
  
}
</style>