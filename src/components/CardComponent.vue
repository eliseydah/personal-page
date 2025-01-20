<template>
  <div class="card">
    <div class="description">
      <img :src="getImageUrl()" class="svg-icon" :alt="title" width="50" height="60" />
      <h3>{{ title }}</h3>
    </div>
    <div>
      <p>{{ description }}</p>
    </div>
    <div class="links">
      <a v-if="linkJs" :href="linkJs">
        <img src="../assets/icons/javascript.svg" width="25" height="25" />
      </a>
      <a v-if="linkVue" :href="linkVue">
        <img src="../assets/icons/vue.svg" width="25" height="25"
      /></a>
    </div>
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  iconFilename: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  linkJs: {
    type: String,
    required: false,
  },
  linkVue: {
    type: String,
    required: false,
  },
})

function getImageUrl() {
  return new URL(`../assets/icons/${props.iconFilename}`, import.meta.url).toString()
}
</script>

<style scoped>
.card {
  background-color: rgba(240, 248, 255, 0.8);
  padding: 1rem 1rem 0.5rem;
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  flex-direction: column;
  border-radius: 5%;
}
h3 {
  font-weight: 500;
}
.links {
  display: flex;
  justify-content: end;
  align-items: end;
}
h3 {
  align-self: center;
}
.description {
  display: flex;
  flex-direction: row;
  justify-content: baseline;
  gap: 1rem;
}
a {
  color: darkblue;
  text-decoration: none;
  padding: 0.5rem 1rem;
  font-weight: 200;
  font-style: italic;
}

a:hover {
  background-color: rgba(240, 248, 255, 0.85);
  border-radius: 10px;
}

.svg-icon {
  filter: invert(47%) sepia(100%) saturate(719%) hue-rotate(180deg) brightness(85%) contrast(91%);
}
</style>
