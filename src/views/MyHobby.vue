<script setup lang="ts">
import HeaderSection from '@/modules/shared/components/HeaderSection.vue'
import FooterSection from '@/modules/shared/components/FooterSection.vue'
import IntroductionHobby from '@/modules/hobby/components/IntroductionHobby.vue'
</script>
<template>
  <div class="landing">
    <HeaderSection></HeaderSection>
    <IntroductionHobby></IntroductionHobby>
  </div>
  <p>hello Artem</p>
  <FooterSection></FooterSection>
</template>
<style scoped>
.landing {
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
    url(../assets/forests.jpg) no-repeat center center;
  background-size: cover;
}
</style>
