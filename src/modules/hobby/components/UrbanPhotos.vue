<script setup lang="ts">
import PhotoCarousel from '@/modules/hobby/components/PhotoCarousel.vue'
import SignComponent from '@/modules/shared/components/SignComponent.vue'
const photos = [
  {
    url: new URL(`../../../assets/urban/01.jpg`, import.meta.url).toString(),
    id: '01',
  },
  {
    url: new URL(`../../../assets/urban/02.jpg`, import.meta.url).toString(),
    id: '02',
  },
  {
    url: new URL(`../../../assets/urban/05.jpg`, import.meta.url).toString(),
    id: '03',
  },
  {
    url: new URL(`../../../assets/urban/04.jpg`, import.meta.url).toString(),
    id: '04',
  },
  {
    url: new URL(`../../../assets/urban/06.jpg`, import.meta.url).toString(),
    id: '05',
  },
  {
    url: new URL(`../../../assets/urban/07.jpg`, import.meta.url).toString(),
    id: '06',
  },
  {
    url: new URL(`../../../assets/urban/08.jpg`, import.meta.url).toString(),
    id: '07',
  },
  {
    url: new URL(`../../../assets/urban/01.jpg`, import.meta.url).toString(),
    id: '08',
  },
  {
    url: new URL(`../../../assets/urban/09.jpg`, import.meta.url).toString(),
    id: '09',
  },
  {
    url: new URL(`../../../assets/urban/04.jpg`, import.meta.url).toString(),
    id: '10',
  },
]
</script>
<template>
  <SignComponent msg="Urban Photo"></SignComponent>
  <PhotoCarousel :photos="photos"></PhotoCarousel>
</template>
<style scoped></style>
