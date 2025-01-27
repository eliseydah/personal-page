<script setup lang="ts">
const props = defineProps({
  iconFilename: {
    type: String,
    required: true,
  },
})

function getImageUrl() {
  return new URL(`../../../assets/icons/${props.iconFilename}`, import.meta.url).toString()
}
</script>
<template>
  <div>
    <a href=""> <img :src="getImageUrl()" class="svg-icon" width="30" height="30" /></a>
  </div>
</template>
<style scoped>
img {
  filter: invert(100%);
}

a {
  display: block;
  height: 25px;
}

a:hover {
  color: var(--important-text-color);
}
</style>
