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
  width: 100%;
  min-height: 100vh;
  background-color: hsl(257, 40%, 49%);
  background-image: url("@/assets/images/bg-mobile.svg");
  background-repeat: no-repeat;
  background-position: center top;
  background-size: 100vw;
  padding-top: 130px;
  /* background-position: center; */
  
}

@media screen and (min-width: 768px) {
  .hero {
     /* background-image: url("@/assets/images/bg-desktop.svg"); */
     padding-top: 260px;
  }
}

@media screen and (min-width: 1440px) {
 .hero {
    background-image: url("@/assets/images/bg-desktop.svg");
    background-size: cover;
    padding-top: 190px;
    background-position: center;
    padding-inline: 80px;
    
  }
}
</style>