<script setup>
  import IllustrationMockup from "@/assets/images/illustration-mockups.svg"
  import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome"

  import { faFacebook, faTwitter, faInstagram } from "@fortawesome/free-brands-svg-icons"

</script>

<template>
  <div class="hero-content">
    <div class="hero-img">
      <img :src="IllustrationMockup" alt="illustration mockup">
    </div>
    <div class="main-content">
      <h1>Build The Community Your Fans Will Love</h1>
      <p>Huddle re-imagines the way we build communities. You have a voice, but so does your audience. Create connections with your users as you engage in genuine discussion.</p>
      <button>Register</button>
      <div class="socials">
        <div>
          <FontAwesomeIcon :icon="faFacebook" />
        </div>
        <div>
          <FontAwesomeIcon :icon="faTwitter" />
        </div>
        <div>
          <FontAwesomeIcon :icon="faInstagram" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>