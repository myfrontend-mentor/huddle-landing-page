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

h1 {
  font-family: "Poppins", sans-serif;
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

@media screen and (min-width: 768px) {
  .hero-img > img {
    width: 600px;
  }

  .hero-content {
    gap: 120px;
  }

  h1 {
    font-size: 2.5rem;
  }

  .main-content {
    padding-inline: 60px;
  }

  p {
    font-size: 1.6rem;
    margin-block: 35px;
  }

  button {
    font-size: 16px;
    width: 280px;
    padding: 12px 18px;
    border-radius: 40px;
    margin-bottom: 100px;
  }
}

@media screen and (min-width: 1440px) {
  .hero-content {
    display: grid;
    grid-template-columns: 1.8fr 1fr;
    align-items: center;
    gap: 60px;
    max-width: 1400px;
    margin: 0 auto;
  }

  .hero-img {
    width: 100%;
  }

  .hero-img > img {
    width: 100%;
    height: auto;
    display: block;
  }


  h1 {
    font-size: 2.4rem;
  }

  .main-content {
    text-align: left;
    padding-inline: 0;
    width: 100%;
  }

  p {
    font-size: 1.125rem;
    margin-block: 25px;
  }

  button {
    font-size: 16px;
    width: 150px;
    padding: 12px 18px;
    border-radius: 40px;
    margin-bottom: 200px;
  }

  .socials {
    justify-content: right;
  }
}
</style>