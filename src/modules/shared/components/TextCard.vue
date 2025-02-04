<script setup lang="ts"></script>
<template>
  <section class="container">
    <div class="box">
      <slot></slot>
    </div>
  </section>
</template>
<style scoped>
.box {
  text-align: center;
  line-height: 50px;
  width: 70%;
  font-size: large;
  background-color: rgba(240, 248, 255, 0.5);
  padding: 1rem 2rem;
}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0rem 0rem 2.5rem;
}
</style>
