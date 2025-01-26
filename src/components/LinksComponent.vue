<!-- todo: remove to SocialsComponent -->
<script setup lang="ts"></script>
<template>
  <section class="links-container">
    <!-- todo: use v-for to render this -->
    <ul>
      <li>
        <a href=""><img src="../assets/icons/github.svg" width="30" height="30" /> </a>
      </li>
      <li>
        <a href=""
          ><img src="../assets/icons/linkedin-round-svgrepo-com.svg" width="30" height="30" />
        </a>
      </li>
      <li>
        <a href=""><img src="../assets/icons/gmail-svgrepo-com.svg" width="30" height="30" /> </a>
      </li>
    </ul>
  </section>
</template>
<style scoped>
ul {
  list-style-type: none;
  display: flex;
  gap: 1rem;
  align-items: center;
}

img {
  filter: invert(100%);
}

a {
  display: block;
  height: 25px;
}

a:hover {
  color: var(--important-text-color);
}
</style>
