<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'
import LinksComponent from '@/modules/shared/components/SocialsLinks.vue'
const currentTime = ref(new Date().toLocaleTimeString('en-US')) // Current time
let timer: number

onMounted(() => {
  timer = setInterval(() => {
    currentTime.value = new Date().toLocaleTimeString('en-US', {
      hour: '2-digit',
      minute: '2-digit',
      hour12: true,
    })
  }, 1000)
})

// clear the timer when the component is unmounted
onUnmounted(() => {
  clearInterval(timer)
})
</script>
<template>
  <div class="line"></div>
  <section class="footer-container">
    <div class="small-footer-container">
      <img src="../../../assets/icons/person.svg" width="25" height="25" />
      <p>Daria Eliseeva</p>
    </div>
    <div class="small-footer-container">
      <img src="../../../assets/icons/clock.svg" width="25" height="25" />
      <span> {{ currentTime }} </span>
    </div>
    <LinksComponent></LinksComponent>
  </section>
</template>
<style scoped>
.footer-container {
  font-size: 1.2rem;
  margin-top: 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: var(--primary-text-color);
}
.small-footer-container {
  display: flex;
  align-items: center;
  gap: 1rem;
}
.line {
  margin-top: 5rem;
  border-bottom: 1px solid var(--primary-text-color);
}
img {
  filter: invert(100%);
}
@media (max-width: 576px) {
  .footer-container {
    display: flex;
    flex-direction: raw;
    flex-wrap: wrap;
  }
}
</style>
