<template>
  <div class="card">
    <div class="description">
      <img :src="getImageUrl()" class="svg-icon" :alt="title" width="50" height="60" />
      <h3>{{ title }}</h3>
    </div>
    <div class="text-description">
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
  background-color: var(--card-bg-color);
  padding: 1rem 1rem 0.5rem;
  display: flex;
  justify-content: space-between;
  gap: 1rem;
  flex-direction: column;
  border-radius: 5%;
}
h3 {
  font-weight: 500;
  color: var(--primary-text-color);
}
.links {
  display: flex;
  justify-content: end;
  align-items: end;
  gap: 0.5rem;
}

.links a {
  filter: invert(100%);
  text-decoration: none;
}

.links a:hover {
  filter: invert(64%) sepia(70%) saturate(502%) hue-rotate(358deg) brightness(110%) contrast(96%);
}

.text-description {
  color: var(--secondary-text-color);
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

.svg-icon {
  filter: invert(45%) sepia(8%) saturate(360%) hue-rotate(205deg) brightness(105%) contrast(99%);
}
</style>
