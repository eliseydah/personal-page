<script setup lang="ts">
import HeaderSection from '@/modules/shared/components/HeaderSection.vue'
import FooterSection from '@/modules/shared/components/FooterSection.vue'
import IntroductionHeader from '@/modules/hobby/components/IntroductionHeader.vue'
import IntroductionHobby from '@/modules/hobby/components/IntroductionHobby.vue'
import PhotoMap from '@/modules/hobby/components/PhotoMap.vue'
</script>
<template>
  <div class="landing">
    <div class="intro">
      <HeaderSection></HeaderSection>
      <IntroductionHeader></IntroductionHeader>
      <IntroductionHobby></IntroductionHobby>
    </div>
    <!-- </div>
  <div class="content"> -->
    <PhotoMap></PhotoMap>
    <FooterSection></FooterSection>
  </div>
</template>
<style scoped>
.intro {
  height: 100vh;
}
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
  background-attachment: fixed;
  background:
    linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url(../assets/forests.jpg) no-repeat center center;
  background-size: cover;
}
</style>
