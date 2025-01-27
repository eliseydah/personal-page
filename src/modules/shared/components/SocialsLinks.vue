<script setup lang="ts">
import SocialIcon from './SocialIcon.vue'
const socialIcons = [
  {
    iconFilename: 'github.svg',
    title: 'GitHub',
  },
  { iconFilename: 'linkedin-round-svgrepo-com.svg', title: 'LinkedIn' },
  { iconFilename: 'gmail-svgrepo-com.svg', title: 'Gmail' },
]
</script>
<template>
  <section class="links-container">
    <SocialIcon
      v-for="item in socialIcons"
      :key="item.title"
      :iconFilename="item.iconFilename"
    ></SocialIcon>
  </section>
</template>
<style scoped>
.links-container {
  display: flex;
  gap: 1rem;
  align-items: center;
}
</style>
