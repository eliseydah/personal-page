<script setup lang="ts">
import CardComponent from './CardComponent.vue'
</script>
<template>
  <section>
    <p class="title">Services area</p>
  </section>
  <div class="card-container">
    <CardComponent
      iconFilename="message.svg"
      title="To-do list"
      description="A simple application for managing task lists. Allows you to add, delete and mark tasks as completed."
      link="https://github.com/eliseydah/todo-js/tree/master/todo"
    />
    <div class="card">
      <div class="description">
        <img src="../assets/icons/message.svg" class="svg-icon" alt="" width="50" height="60" />
        <h3>Chat page</h3>
        <p>
          A simple application that simulates chat functionality, showcasing only the frontend
          without any backend integration.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/chat">go to Chat page</a>
      </div>
    </div>
    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Wheel of fortune</h3>
        <p>
          This is interactive web application where users can spin a Wheel of Fortune to receive a
          name of the city as an idea to visit.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/fortune"
          >go to Wheel of fortune</a
        >
      </div>
    </div>

    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Wishlist</h3>
        <p>
          A simple application for creating a list of wishes. It allows you to create a wish card,
          describe a wish, upload a picture, add a link, and delete the wish card.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/wishlist"> go to wishlist</a>
      </div>
    </div>
    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Weather widget</h3>
        <p>A simple web-page which allows to search a weather.</p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/weather">go to the vue chat</a>
      </div>
    </div>
    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>A layout training</h3>
        <p>
          A simple application for creating a list of wishes. It allows you to create a wish card,
          describe a wish, upload a picture, add a link, and delete the wish card.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/landing"> to layout</a>
      </div>
    </div>
    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Vue to-do list</h3>
        <p>
          A simple application for managing task lists. Allows you to add, delete and mark tasks as
          completed.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-todo">
          go to vue to-do list</a
        >
      </div>
    </div>
    <div class="card">
      <div class="description">
        <img src="./forest.jpg" alt="" width="50" height="60" />
        <h3>Vue chat</h3>
        <p>
          A simple application that simulates chat functionality, showcasing only the frontend
          without any backend integration.
        </p>
      </div>
      <div class="forLink">
        <a href="https://github.com/eliseydah/todo-js/tree/master/vue-chat"> go to the vue chat</a>
      </div>
    </div>
    <div class="card">
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
  padding: 1rem 1rem 0.5rem;
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  flex-direction: column;
}
h3 {
  font-weight: 500;
}
.forLink {
  display: flex;
  justify-content: end;
  align-items: end;
}
a {
  color: darkblue;
  text-decoration: none;
  padding: 0.5rem 1rem;
  font-weight: 200;
  font-style: italic;
}

a:hover {
  background-color: rgba(240, 248, 255, 0.295);
  border-radius: 10px;
}

.svg-icon {
  filter: invert(27%) sepia(100%) saturate(7496%) hue-rotate(180deg) brightness(95%) contrast(101%);
}
</style>
