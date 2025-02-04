<script setup lang="ts"></script>
<template>
  <section class="container">
    <p>my hobbies</p>
    <div class="line"></div>
  </section>
</template>
<style scoped>
p {
  text-transform: uppercase;
  font-size: 5rem;
  font-weight: bold;
  color: var(--primary-text-color);
  opacity: 0.5;
  letter-spacing: 0.2rem;
}
.line {
  margin-top: 1rem;
  width: 30%;
  border-bottom: 2px solid var(--primary-text-color);
  opacity: 0.5;
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 10rem 0rem 3rem;
}
</style>
