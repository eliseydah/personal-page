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
      <li><span>My Number</span></li>
    </ul>
  </section>
</template>
<style scoped>
.main {
  /* padding: 0rem, 2rem; */
  display: flex;
  /* flex-direction: raw;
  justify-content: space-between; */
  /* color: darkblue; */
}
.container {
  width: 100%;
  margin-top: 1.5rem;
  display: flex;
  flex-direction: raw;
  justify-content: center;
  align-items: flex-end;
  gap: 4rem;
  list-style-type: none;
}
a,
span {
  color: darkblue;
  text-decoration: none;
  padding: 1rem 3rem;
}

a:hover {
  background-color: rgba(240, 248, 255, 0.295);
  border-radius: 10px;
}
</style>
