<script setup lang="ts">
import IntroductionSection from '@/modules/job/components/IntroductionSection.vue'
import HeaderSection from '@/modules/shared/components/HeaderSection.vue'
import AboutMeSection from '@/modules/job/components/AboutMeSection.vue'
import ServicesSection from '@/modules/job/components/ServicesSection.vue'
import LanguagesAndToolsSection from '@/modules/job/components/LanguagesAndToolsSection.vue'
import FooterSection from '@/modules/shared/components/FooterSection.vue'
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
