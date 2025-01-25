<script setup lang="ts">
import SignComponent from './SignComponent.vue'
</script>
<template>
  <span id="about-me"></span>
  <SignComponent msg="ABOUT ME"></SignComponent>
  <section>
    <div class="contain">
      <div>
        <img src="../assets/forests.jpg" width="250" height="300" />
      </div>
      <div class="text-box">
        <h3>Hi there! I'm Daria Eliseeva</h3>
        <h5>Frontend Developer</h5>
        <section class="main-text">
          <p>Birthday: <span>16.12.1998</span></p>
          <p>Phone: <span></span></p>
          <p>E-mail: <span> eliseydah@gmail.com</span></p>
          <p>Live in: <span> Berlin</span></p>
          <p>Language:<span> English, Russian</span></p>
          <button class="downloadCv">Resume</button>
        </section>
      </div>
    </div>
  </section>
</template>
<style>
.contain {
  font-size: 1.5rem;
  background-color: var(--card-bg-color);
  padding: 3rem 3rem;
  display: flex;
  /* gap: 2rem; */
  box-sizing: content-box;
  justify-content: space-around;
  align-items: center;
  /* height: 50vh; */
}
.text-box {
  display: flex;
  color: var(--secondary-text-color);
  flex-direction: column;
  font-size: 1.2rem;
}
.downloadCv {
  margin-top: 2rem;
  width: 10rem;
  padding: 1rem 3rem;
  background-color: var(--important-text-color);
  color: black;
  border: 0;
  border-radius: 2rem;
}
.downloadCv:hover {
  background-color: rgba(240, 248, 255, 0.65);
}
h3 {
  align-self: center;
  font-size: 2rem;
  color: var(--primary-text-color);
}
h5 {
  font-size: 1.5rem;
  color: var(--important-text-color);
  font-weight: bold;
}
@media (max-width: 576px) {
  .contain {
    display: flex;
    flex-direction: column;
  }
}
</style>
