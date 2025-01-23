<script setup lang="ts"></script>
<template>
  <span id="home"></span>
  <section class="container">
    <div class="box">
      <h1>HI! I am Daria Eliseeva</h1>
      <p>
        I’m a frontend developer specializing in creating modern, responsive, and creative web
        applications. My goal is to turn your ideas into beautiful and functional websites that
        impress and work seamlessly across all devices. Here, you’ll find information about me, my
        projects, and ways to get in touch.
      </p>
    </div>
  </section>
</template>
<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  /* height: 90vh; */
}
p {
  line-height: 2rem;
}
.box {
  text-align: center;
  line-height: 50px;
  width: 70%;
  font-size: large;
  background-color: rgba(240, 248, 255, 0.5);
  padding: 1rem 2rem;
}
@media (max-width: 576px) {
  .container {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
}
</style>
