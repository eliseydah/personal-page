<script setup lang="ts">
import SignComponent from './SignComponent.vue'
</script>
<template>
  <span id="about-me"></span>
  <SignComponent msg="about me"></SignComponent>
  <section>
    <div class="about-me-container">
      <div>
        <img src="../assets/forests.jpg" width="250" height="300" />
      </div>
      <div class="text-box">
        <p class="greetings">Hi there! I'm Daria Eliseeva</p>
        <p class="main-info">Frontend Developer</p>
        <section class="main-text">
          <p>Birthday: <span>16.12.1998</span></p>
          <p>Phone: <span></span></p>
          <p>E-mail: <span> eliseydah@gmail.com</span></p>
          <p>Live in: <span> Berlin</span></p>
          <p>Language:<span> English, Russian</span></p>
          <button class="download-cv">Resume</button>
        </section>
      </div>
    </div>
  </section>
</template>
<style>
.about-me-container {
  font-size: 1.5rem;
  background-color: var(--card-bg-color);
  padding: 3rem 3rem;
  display: flex;
  box-sizing: content-box;
  justify-content: space-around;
  align-items: center;
}
.text-box {
  display: flex;
  color: var(--secondary-text-color);
  flex-direction: column;
  font-size: 1.2rem;
}
.download-cv {
  margin-top: 2rem;
  width: 10rem;
  padding: 1rem 3rem;
  background-color: var(--important-text-color);
  color: black;
  border: 0;
  border-radius: 2rem;
}
.download-cv:hover {
  background-color: var(--secondary-text-color);
}
.greetings {
  align-self: center;
  font-size: 2rem;
  color: var(--primary-text-color);
}
.main-info {
  font-size: 1.5rem;
  color: var(--important-text-color);
  font-weight: bold;
}
@media (max-width: 576px) {
  .about-me-container {
    display: flex;
    flex-direction: column;
  }
}
</style>
