<script setup lang="ts">
import LinksComponent from './SocialsComponent.vue'
</script>

<template>
  <section class="main">
    <ul class="header-container">
      <li><a href="#home">HOME</a></li>
      <li><a href="#about-me">ABOUT ME</a></li>
      <li><a href="#my-projects">MY PROJECTS</a></li>
      <li><a href="#skills">SKILLS</a></li>
    </ul>
    <LinksComponent class="socials"></LinksComponent>
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
}

a:hover {
  color: var(--important-text-color);
}

@media (max-width: 576px) {
  .header-container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: flex-start;
    align-items: flex-start;
  }
  .main {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    margin-bottom: 50px;
    align-items: end;
  }

  .socials {
    align-items: flex-end;
  }
}
</style>
