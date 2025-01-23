<script setup lang="ts">
import IntroductionSection from './components/IntroductionSection.vue'
import HeaderSection from './components/HeaderSection.vue'
import AboutMeSection from './components/AboutMeSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import LanguagesAndToolsSection from './components/LanguagesAndToolsSection.vue'
import FooterSection from './components/FooterSection.vue'
</script>

<template>
  <div class="face-page">
    <HeaderSection></HeaderSection>
    <IntroductionSection></IntroductionSection>
  </div>
  <div class="continuation">
    <AboutMeSection></AboutMeSection>
    <ServicesSection></ServicesSection>
    <LanguagesAndToolsSection></LanguagesAndToolsSection>
    <FooterSection></FooterSection>
  </div>
  <!-- We don't need router yet -->
  <!-- <RouterView /> -->
</template>

<style scoped>
.face-page {
  background-image: url(./assets//mountains.jpg);
  background-repeat: no-repeat;
  background-position: center center;
  background-attachment: fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  width: 100vw;
  height: 100vh;
}
.continuation {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;
}
</style>
