<script setup lang="ts">
import PhotoCarousel from '@/modules/hobby/components/PhotoCarousel.vue'
import SignComponent from '@/modules/shared/components/SignComponent.vue'
import TextCard from '@/modules/shared/components/TextCard.vue'
const photos = [
  {
    url: new URL(`../../../assets/sport/1.jpg`, import.meta.url).toString(),
    id: '01',
  },
  {
    url: new URL(`../../../assets/sport/2.jpg`, import.meta.url).toString(),
    id: '02',
  },
  {
    url: new URL(`../../../assets/sport/3.jpg`, import.meta.url).toString(),
    id: '03',
  },
  {
    url: new URL(`../../../assets/sport/4.jpg`, import.meta.url).toString(),
    id: '04',
  },
  {
    url: new URL(`../../../assets/sport/5.jpg`, import.meta.url).toString(),
    id: '05',
  },
  {
    url: new URL(`../../../assets/sport/6.jpg`, import.meta.url).toString(),
    id: '06',
  },
]
</script>
<template>
  <SignComponent msg="My Sports activities"></SignComponent>
  <TextCard>
    <p>
      I love sports and outdoor activities. They help me stay healthy, active, and energized. I
      enjoy hiking, practicing pilates, and playing volleyball.Sports are not only a great way to
      stay in shape but also a way to relax, clear my mind, and enjoy the beauty of nature. I
      believe that a healthy body leads to a healthy mind, and sports are an essential part of my
      life.
    </p>
  </TextCard>
  <PhotoCarousel :photos="photos"></PhotoCarousel>
</template>
<style scoped>
p {
  line-height: 2rem;
}
</style>
