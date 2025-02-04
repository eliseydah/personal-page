<script setup lang="ts">
import PhotoCarousel from '@/modules/hobby/components/PhotoCarousel.vue'
import SignComponent from '@/modules/shared/components/SignComponent.vue'
const photos = [
  {
    url: new URL(`../../../assets/nature/IMG_01.JPG`, import.meta.url).toString(),
    id: '01',
  },
  {
    url: new URL(`../../../assets/nature/IMG_02.JPG`, import.meta.url).toString(),
    id: '02',
  },
  {
    url: new URL(`../../../assets/nature/IMG_03.JPG`, import.meta.url).toString(),
    id: '03',
  },
  {
    url: new URL(`../../../assets/nature/IMG_04.JPG`, import.meta.url).toString(),
    id: '04',
  },
  {
    url: new URL(`../../../assets/nature/IMG_05.JPG`, import.meta.url).toString(),
    id: '05',
  },
  {
    url: new URL(`../../../assets/nature/IMG_06.JPG`, import.meta.url).toString(),
    id: '06',
  },
  {
    url: new URL(`../../../assets/nature/IMG_07.JPG`, import.meta.url).toString(),
    id: '07',
  },
  {
    url: new URL(`../../../assets/nature/IMG_08.JPG`, import.meta.url).toString(),
    id: '08',
  },
  {
    url: new URL(`../../../assets/nature/IMG_09.JPG`, import.meta.url).toString(),
    id: '09',
  },
  {
    url: new URL(`../../../assets/nature/IMG_10.JPG`, import.meta.url).toString(),
    id: '10',
  },
]
</script>
<template>
  <SignComponent msg="Nature Photo"></SignComponent>
  <PhotoCarousel :photos="photos"></PhotoCarousel>
  <SignComponent msg="Urban Photo"></SignComponent>
  <PhotoCarousel :photos="photos"></PhotoCarousel>
</template>
<style scoped></style>
