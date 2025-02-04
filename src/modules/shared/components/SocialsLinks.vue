<script setup lang="ts">
import SocialIcon from './SocialIcon.vue'
const socialIcons = [
  {
    iconFilename: 'github.svg',
    title: 'GitHub',
    link: 'https://github.com/eliseydah',
  },
  {
    iconFilename: 'linkedin-round-svgrepo-com.svg',
    title: 'LinkedIn',
    link: 'https://www.linkedin.com/in/daria-eliseeva-67084234a/',
  },
  { iconFilename: 'gmail-svgrepo-com.svg', title: 'Gmail', link: 'mailto:eliseydah@gmail.com' },
]
</script>
<template>
  <section class="links-container">
    <SocialIcon
      v-for="item in socialIcons"
      :key="item.title"
      :iconFilename="item.iconFilename"
      :link="item.link"
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
