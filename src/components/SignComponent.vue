<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>
<template>
  <section class="container-sign">
    <p class="text-front">{{ msg }}</p>
    <p class="text-back">{{ msg }}</p>
  </section>
</template>
<style scoped>
.container-sign {
  position: relative;
  height: 10vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.text-back {
  position: absolute;
  font-size: 3rem;
  font-weight: bold;
  color: rgba(250, 248, 248, 0.07);
  z-index: 1;
}

.text-front {
  position: absolute;
  font-size: 1.2rem;
  font-weight: bold;
  color: var(--important-text-color);
  z-index: 2;
}
</style>
