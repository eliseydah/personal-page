<script setup lang="ts">
import IntroductionSection from './components/IntroductionSection.vue'
import HeaderSection from './components/HeaderSection.vue'
import AboutMeSection from './components/AboutMeSection.vue'
import ServicesSection from './components/ServicesSection.vue'
</script>

<template>
  <HeaderSection></HeaderSection>
  <IntroductionSection></IntroductionSection>
  <AboutMeSection></AboutMeSection>
  <ServicesSection></ServicesSection>
  <!-- We don't need router yet -->
  <!-- <RouterView /> -->
</template>

<style scoped></style>
