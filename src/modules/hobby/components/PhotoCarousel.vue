<script setup lang="ts">
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Navigation } from 'vue3-carousel'
defineProps({
  photos: {
    type: Array<{
      id: string | number
      url: string
    }>,
    required: true,
  },
})

const config = {
  height: 500,
  itemsToShow: 4,
  gap: 3,
  wrapAround: true,
}
</script>

<template>
  <Carousel v-bind="config">
    <Slide v-for="image in photos" :key="image.id">
      <img :src="image.url" width="400" height="600" alt="image" />
    </Slide>

    <template #addons>
      <Navigation />
    </template>
  </Carousel>
</template>
