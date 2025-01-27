<script setup lang="ts">
import IntroductionSection from './components/IntroductionSection.vue'
import HeaderSection from './components/HeaderSection.vue'
import AboutMeSection from './components/AboutMeSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import LanguagesAndToolsSection from './components/LanguagesAndToolsSection.vue'
import FooterSection from './components/FooterSection.vue'
</script>

<template>
  <div class="landing">
    <HeaderSection></HeaderSection>
    <IntroductionSection></IntroductionSection>
  </div>
  <div class="content">
    <AboutMeSection></AboutMeSection>
    <ServicesSection></ServicesSection>
    <LanguagesAndToolsSection></LanguagesAndToolsSection>
    <FooterSection></FooterSection>
  </div>
  <!-- We don't need router yet -->
  <!-- <RouterView /> -->
</template>

<style scoped>
.landing {
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

  background:
    linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url(./assets//mountains.jpg) no-repeat center center;
  background-size: cover;
}

.content {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;
}
</style>
