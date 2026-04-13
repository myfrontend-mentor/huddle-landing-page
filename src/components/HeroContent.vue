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
.hero-content {
  /*  */
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 60px;
}

.hero-img > img {
  width: 310px;
}

.main-content {
  text-align: center;
  padding-inline: 30px;
}

p {
  /* font-size: 18px; */
  margin-block: 25px;
}

button {
  font-size: 14px;
  border: none;
  background: white;
  color: hsl(257, 40%, 49%);
  width: 200px;
  padding: 9px 18px;
  border-radius: 40px;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  cursor: pointer;
  margin-bottom: 80px;
}

.socials {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  margin-bottom: 50px;
}

.socials > div {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 30px;
  height: 30px;
  border: 1px solid white;
  border-radius: 50%;
}

button:hover {
  background: hsl(300, 69%, 71%);
  color: white;
}

.socials > div:hover {
  border: 1px solid hsl(300, 69%, 71%);
  cursor: pointer;
  color: hsl(300, 69%, 71%);
}
</style>