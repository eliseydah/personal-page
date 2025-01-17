<template>
  <div class="card">
    <div class="description">
      <img :src="getImageUrl()" class="svg-icon" :alt="title" width="50" height="60" />
      <h3>{{ title }}</h3>
      <p>{{ description }}</p>
    </div>
    <div class="forLink">
      <a :href="link">go to {{ title }}</a>
    </div>
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  iconFilename: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  link: {
    type: String,
    required: true,
  },
})

function getImageUrl() {
  return new URL(`../assets/icons/${props.iconFilename}`, import.meta.url)
}
</script>

<style scoped>
/* Add your styles here */
</style>
