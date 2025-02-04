<script setup lang="ts">
import HeaderSection from '@/modules/shared/components/HeaderSection.vue'
import FooterSection from '@/modules/shared/components/FooterSection.vue'
import IntroductionHeader from '@/modules/hobby/components/IntroductionHeader.vue'
import NaturePhotos from '@/modules/hobby/components/NaturePhotos.vue'
import UrbanPhotos from '@/modules/hobby/components/UrbanPhotos.vue'
import SportSection from '@/modules/hobby/components/SportSection.vue'
import TextCard from '@/modules/shared/components/TextCard.vue'
</script>
<template>
  <div class="landing">
    <div class="intro">
      <HeaderSection></HeaderSection>
      <IntroductionHeader></IntroductionHeader>
      <TextCard>
        <p>
          Everyone has a passion that brings them joy and inspiration. My hobby is nature
          photography. I love capturing beautiful landscapes, the play of light and shadow, the
          change of seasons, and unique moments that nature gives us. Photography helps me see the
          world in a new way and appreciate its beauty.
        </p>
        <p>
          I also enjoy urban photography, capturing the energy of city streets, modern architecture,
          and the contrast between nature and urban life. Every city has its own character, and
          through my photos, I try to show its unique atmosphere and hidden beauty.
        </p>
      </TextCard>
    </div>
    <NaturePhotos></NaturePhotos>
    <UrbanPhotos></UrbanPhotos>
    <SportSection></SportSection>
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
p {
  line-height: 2rem;
}
@media (max-width: 576px) {
  .intro {
    height: auto;
  }
}
</style>
