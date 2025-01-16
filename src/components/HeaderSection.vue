<script setup lang="ts"></script>

<template>
  <section class="main">
    <!-- <img alt="Vue logo" class="logo" src="@/assets/mountains.jpg" width="125" height="125" /> -->

    <ul class="container">
      <li><a href="">HOME</a></li>
      <li><a href="">ABOUT</a></li>
      <li><a href="">RESUME</a></li>
      <li><a href="">PORTFOLIO</a></li>
      <li><a href="">CONTACT</a></li>
    </ul>
    <p>My Number</p>
  </section>
</template>
<style scoped>
.main {
  padding: 0rem, 2rem;
  display: flex;
  flex-direction: raw;
  justify-content: space-between;
  color: darkblue;
}
.container {
  display: flex;
  flex-direction: raw;
  gap: 4rem;
  list-style-type: none;
}
a {
  color: darkblue;
  text-decoration: none;
  padding: 1rem 3rem;
}

a:hover {
  background-color: rgba(3, 33, 43, 0.101);
  border-radius: 10px;
}
</style>
