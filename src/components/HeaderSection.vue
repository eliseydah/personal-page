<script setup lang="ts">
import LinksComponent from './LinksComponent.vue'
</script>

<template>
  <section class="main">
    <ul class="header-container">
      <li><a href="#home">HOME</a></li>
      <li><a href="#about-me">ABOUT ME</a></li>
      <li><a href="#my-projects">MY PROJECTS</a></li>
      <li><a href="#skills">SKILLS</a></li>
    </ul>
    <LinksComponent class="links"></LinksComponent>
  </section>
</template>
<style scoped>
.main {
  width: 100%;
  padding-top: 1.5rem;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.header-container {
  /* width: 100%; */
  /* margin-top: 1.5rem; */
  display: flex;
  flex-direction: raw;
  justify-content: center;
  align-items: flex-end;
  gap: 4rem;
  list-style-type: none;
}
a,
span {
  color: var(--primary-text-color);
  text-decoration: none;
  font-size: 1.2rem;
  /* padding: 1rem 3rem; */
}

a:hover {
  color: var(--important-text-color);
}
</style>
