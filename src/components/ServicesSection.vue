<script setup lang="ts">
import CardComponent from './CardComponent.vue'
const cards = [
  {
    iconFilename: 'list.svg',
    title: 'To-do list',
    description:
      'A simple application for managing task lists. Allows you to add, delete and mark tasks as completed.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/todo',
    linkVue: 'https://github.com/eliseydah/todo-js/tree/master/vue-todo',
  },
  {
    iconFilename: 'message.svg',
    title: 'Chat page',
    description:
      'A simple application that simulates chat functionality, showcasing only the frontend without any backend integration.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/chat',
    linkVue: 'https://github.com/eliseydah/todo-js/tree/master/vue-chat',
  },
  {
    iconFilename: 'wheel.svg',
    title: 'Wheel of fortune',
    description:
      'This is interactive web application where users can spin a Wheel of Fortune to receive a name of the city as an idea to visit.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/fortune',
  },
  {
    iconFilename: 'wish.svg',
    title: 'Wishlist',
    description:
      'A simple application for creating a list of wishes. It allows you to create a wish card, describe a wish, upload a picture, add a link, and delete the wish card.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/wishlist',
    linkVue: 'https://github.com/eliseydah/todo-js/tree/master/vue-wishlist',
  },
  {
    iconFilename: 'weather.svg',
    title: 'Weather widget',
    description: 'A simple web-page which allows to search a weather.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/weather',
    linkVue: 'https://github.com/eliseydah/todo-js/tree/master/vue-weather-widget',
  },
  {
    iconFilename: 'layout.svg',
    title: 'A layout training',
    description:
      'A simple application for creating a list of wishes. It allows you to create a wish card, describe a wish, upload a picture, add a link, and delete the wish card.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/landing',
  },
]
</script>
<template>
  <section>
    <p class="title">Services area</p>
  </section>
  <div class="card-container">
    <CardComponent
      v-for="card in cards"
      :key="card.title"
      :title="card.title"
      :description="card.description"
      :iconFilename="card.iconFilename"
      :link-js="card.linkJS"
      :link-vue="card.linkVue"
    />

    <!-- <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Vue Wishlist</h3>
        <p>
          A simple application for creating a list of wishes. It allows you to create a wish card,
          describe a wish, upload a picture, add a link, and delete the wish card.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-wishlist">
          go to vue wishlist</a
        >
      </div>
    </div>
    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Vue Weather widget</h3>
        <p>A simple web-page which allows to search a weather.</p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-weather-widget">
          go to vue weather widget</a
        >
      </div>
    </div> -->
  </div>
</template>
<style scoped>
.card-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  width: 100%;
  flex-wrap: wrap;
  /* justify-content: space-around; */
  gap: 1rem;
  margin-top: 1rem;
}
</style>
