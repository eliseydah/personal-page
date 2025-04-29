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
    linkReact: 'https://github.com/eliseydah/my-projects/tree/master/react/react-todo',
  },
  {
    iconFilename: 'message.svg',
    title: 'Chat page',
    description:
      'A simple application that simulates chat functionality, showcasing only the frontend without any backend integration.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/chat',
    linkVue: 'https://github.com/eliseydah/todo-js/tree/master/vue-chat',
    linkReact: 'https://github.com/eliseydah/my-projects/tree/master/react/react-chat',
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
    linkReact: 'https://github.com/eliseydah/my-projects/tree/master/react/react-wishlist',
  },
  {
    iconFilename: 'weather.svg',
    title: 'Weather widget',
    description: 'A simple web-page which allows to search a weather.',
    linkJS: 'https://github.com/eliseydah/todo-js/tree/master/weather',
    linkVue: 'https://github.com/eliseydah/todo-js/tree/master/vue-weather-widget',
    linkReact: 'https://github.com/eliseydah/my-projects/tree/master/react/react-weather',
  },
  {
    iconFilename: 'plant.svg',
    title: 'Plants shop',
    description:
      'A plant shop web page where users can choose plants, view detailed information about each one, and add favorites.The plants are also organized into several sections, allowing users to easily find a category that suits their needs.',
    linkReact: 'https://github.com/eliseydah/my-projects/tree/master/react/react-plants',
  },
  {
    iconFilename: 'kotlin.svg',
    title: 'Lotto game',
    description:
      'An application that simulates a lottery game. The user can enter an amount to buy tickets (divisible by 1,000), choose their winning numbers, and provide a bonus number. The program calculates how many numbers match in the purchased tickets and displays the winning results and total profit.',
    linkKotlin: 'https://github.com/eliseydah/kotlin-lotto-precourse/tree/eliseydah',
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
      :link-react="card.linkReact"
      :link-kotlin="card.linkKotlin"
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
