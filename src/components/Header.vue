<script setup>
</script>

<template>
  <header class="header">
    <div class="header-container">
      <img src="@/assets/images/logo.svg" alt="logo">
    </div>
  </header>
</template>

<style scoped>
.header {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 10;
  background: transparent;
}



header {
  padding: 30px 40px;
}

.header-container {
  max-width: 1300px;
} 

img {
  width: 130px;
}

@media screen and (min-width: 768px) {
  header {
    padding: 60px 80px;
  } 

  img {
    width: 250px;
  }
}

@media secreen and (min-width: 1440px) {
  .header-container {
  max-width: 1400px;      
  margin: 0 auto;         
  padding-block: 40px; 
}
}
</style>