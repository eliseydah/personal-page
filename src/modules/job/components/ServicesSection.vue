<script setup lang="ts">
import SignComponent from '@/modules/shared/components/SignComponent.vue'
import CardComponent from '@/modules/job/components/CardComponent.vue'
const cards = [
  {
    iconFilename: 'ledder.svg',
    title: 'Scaffolding Management',
    description:
      'This app provide basic functionalities to manage a very specific scaffolding business. The functionality basically includes client management and invoice management',
    linkVue: 'https://github.com/fr-ser/scaffolding-management',
  },
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
    title: 'Layout training',
    description:
      'A simple application for creating a list of wishes. It allows you to create a wish card, describe a wish, upload a picture, add a link, and delete the wish card.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/landing',
  },
]
</script>
<template>
  <section>
    <span id="my-projects"></span>
    <SignComponent msg="my projects" />
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
  </div>
</template>
<style scoped>
.card-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  width: 100%;
  flex-wrap: wrap;
  gap: 1rem;
  margin-top: 1rem;
}
@media (max-width: 576px) {
  .card-container {
    display: flex;
    flex-direction: column;
  }
}
</style>
