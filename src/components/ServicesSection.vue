<script setup lang="ts"></script>
<template>
  <section>
    <p class="title">Services area</p>
  </section>
  <div class="card-container">
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>To-do list</h3>
      <p>
        A simple application for managing task lists. Allows you to add, delete and mark tasks as
        completed.
      </p>
      <p><a href="">go to To-do list </a></p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Chat page</h3>
      <p>
        A simple application that simulates chat functionality, showcasing only the frontend without
        any backend integration.
      </p>
      <p><a href="https://github.com/eliseydah/todo-js/tree/master/chat">go to Chat page</a></p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Wheel of fortune</h3>
      <p>
        This is interactive web application where users can spin a Wheel of Fortune to receive a
        name of the city as an idea to visit.
      </p>
      <p>
        <a href="https://github.com/eliseydah/todo-js/tree/master/fortune"
          >go to Wheel of fortune</a
        >
      </p>
    </div>

    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Wishlist</h3>
      <p>
        A simple application for creating a list of wishes. It allows you to create a wish card,
        describe a wish, upload a picture, add a link, and delete the wish card.
      </p>
      <p><a href="https://github.com/eliseydah/todo-js/tree/master/wishlist"> go to wishlist</a></p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Weather widget</h3>
      <p>A simple web-page which allows to search a weather.</p>
      <p>
        <a href="https://github.com/eliseydah/todo-js/tree/master/weather"></a> go to the vue chat
      </p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>A layout training</h3>
      <p>
        A simple application for creating a list of wishes. It allows you to create a wish card,
        describe a wish, upload a picture, add a link, and delete the wish card.
      </p>
      <p><a href="https://github.com/eliseydah/todo-js/tree/master/landing"> to layout</a></p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Vue to-do list</h3>
      <p>
        A simple application for managing task lists. Allows you to add, delete and mark tasks as
        completed.
      </p>
      <p>
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-todo">
          go to vue to-do list</a
        >
      </p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Vue chat</h3>
      <p>
        A simple application that simulates chat functionality, showcasing only the frontend without
        any backend integration.
      </p>
      <p>
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-chat"></a> go to the vue chat
      </p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Vue Wishlist</h3>
      <p>
        A simple application for creating a list of wishes. It allows you to create a wish card,
        describe a wish, upload a picture, add a link, and delete the wish card.
      </p>
      <p>
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-wishlist">
          go to vue weather widget</a
        >
      </p>
    </div>
    <div class="card">
      <img src="./forest.jpg" alt="" width="50" height="60" />
      <h3>Vue Weather widget</h3>
      <p>A simple web-page which allows to search a weather.</p>
      <p>
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-weather-widget">
          go to vue weather widget</a
        >
      </p>
    </div>
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
.card {
  background-color: rgba(240, 248, 255, 0.35);
  padding: 1rem 1rem;
}
</style>
