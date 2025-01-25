<script setup lang="ts">
import SignComponent from './SignComponent.vue'
</script>
<template>
  <span id="skills"></span>
  <SignComponent msg="LANGUAGES AND TOOLS"></SignComponent>
  <section class="icons">
    <img src="../assets/icons/javascript.svg" width="40" height="40" />
    <img src="../assets/icons/vue.svg" width="40" height="40" />
    <img src="../assets/icons/css.svg" width="40" height="40" />
    <img src="../assets/icons/html5.svg" width="40" height="40" />
    <img src="../assets/icons/tailwind.svg" width="40" height="40" />
    <img src="../assets/icons/git.svg" width="40" height="40" />
    <img src="../assets/icons/typescript.svg" width="40" height="40" />
    <img src="../assets/icons/nodejs.svg" width="40" height="40" />
  </section>
</template>
<style scoped>
.icons {
  filter: invert(100%);
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
}
@media (max-width: 576px) {
  .icons {
    display: flex;
    flex-direction: raw;
    flex-wrap: wrap;
  }
}
</style>
