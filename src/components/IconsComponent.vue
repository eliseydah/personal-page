<script setup lang="ts">
const props = defineProps({
  iconFilename: {
    type: String,
    required: true,
  },
})

function getImageUrl() {
  return new URL(`../assets/icons/${props.iconFilename}`, import.meta.url).toString()
}
</script>
<template>
  <div><img :src="getImageUrl()" class="svg-icon" width="50" height="60" /></div>
</template>
<style scoped></style>
