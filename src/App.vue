<template>
  <div id="app">
    <div class="container">
      <HeaderSb />
      <Herosb />
      <GridCardsSec />
      <TipsTricksSec />
      <BizFeaturesSec />
      <TestimonialsSec />
      <ContactFormSec />
      <PostsSec />
      <FooterSb />
    </div>
  </div>
</template>

<script>
import HeaderSb from './components/HeaderSb.vue';
import Herosb from './components/HeroSb.vue';
import GridCardsSec from './components/GridCardsSec.vue';
import TipsTricksSec from './components/TipsTricksSec.vue';
import BizFeaturesSec from './components/BizFeaturesSec.vue';
import TestimonialsSec from './components/TestimonialsSec.vue';
import PostsSec from './components/PostsSec.vue';
import ContactFormSec from './components/ContactFormSec.vue';
import FooterSb from './components/FooterSb.vue';

export default {
  name: 'App',
  components: {
    HeaderSb,
    Herosb,
    GridCardsSec,
    TipsTricksSec,
    BizFeaturesSec,
    TestimonialsSec,
    PostsSec,
    ContactFormSec,
    FooterSb,
  }
}
</script>

<style lang="scss">
@import "@/assets/styles/style.scss";
</style>
