<script setup lang="ts">
import 'vue3-carousel/dist/carousel.css'
import { ref, computed, onMounted, onUnmounted } from 'vue'
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

const screenWidth = ref(window.innerWidth)

const config = computed(() => ({
  height: 500,
  itemsToShow: screenWidth.value < 576 ? 1 : screenWidth.value < 992 ? 2 : 4,
  gap: screenWidth.value < 576 ? 2 : screenWidth.value < 992 ? 3 : 5,
  wrapAround: true,
}))

function updateScreenWidth() {
  screenWidth.value = window.innerWidth
}

onMounted(() => {
  window.addEventListener('resize', updateScreenWidth)
})

onUnmounted(() => {
  window.removeEventListener('resize', updateScreenWidth)
})
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
<style scoped>
@media (max-width: 576px) {
  img {
    width: 100%;
  }
}
</style>
