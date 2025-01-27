<script setup lang="ts">
import SignComponent from '@/modules/shared/components/SignComponent.vue'
import IconComponent from '@/modules/shared/components/IconComponent.vue'
const icons = [
  {
    iconFilename: 'javascript.svg',
    title: 'JavaScript',
  },
  {
    iconFilename: 'vue.svg',
    title: 'Vue',
  },
  {
    iconFilename: 'css.svg',
    title: 'CSS',
  },
  {
    iconFilename: 'html5.svg',
    title: 'HTML5',
  },
  {
    iconFilename: 'tailwind.svg',
    title: 'Tailwind',
  },
  {
    iconFilename: 'git.svg',
    title: 'Git',
  },
  {
    iconFilename: 'typescript.svg',
    title: 'TypeScript',
  },
  {
    iconFilename: 'nodejs.svg',
    title: 'Node.js',
  },
]
</script>
<template>
  <span id="skills"></span>
  <SignComponent msg="languages and tools"></SignComponent>
  <section class="icons">
    <IconComponent
      v-for="item in icons"
      :key="item.title"
      :iconFilename="item.iconFilename"
    ></IconComponent>
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
