<template>
  <div id="app">
    <HeaderComponent :navMenu="navMenu" />

    <main>
      <SpecialistsComponent />
      <PanoramaImage />
      <ExploreComponent />
      <OurCoreComponent />
      <SliderComponent />
      <LatestNewsComponent />
      <TrustedPartnerComponent />
      <CtaImage />
    </main>

    <FooterComponent />
  </div>
</template>

<script>

import HeaderComponent from "./components/HeaderComponent.vue";
import SpecialistsComponent from "./components/SpecialistsComponent.vue";
import PanoramaImage from "./components/PanoramaImage.vue";
import ExploreComponent from "./components/ExploreComponent.vue";
import OurCoreComponent from "./components/OurCoreComponent.vue";
import SliderComponent from "./components/SliderComponent.vue";
import LatestNewsComponent from "./components/LatestNewsComponent.vue";
import TrustedPartnerComponent from "./components/TrustedPartnerComponent.vue";
import CtaImage from "./components/CtaImage.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  name: 'App',
  components: {
   HeaderComponent,
   SpecialistsComponent,
   PanoramaImage,
   ExploreComponent,
   OurCoreComponent,
   SliderComponent,
   LatestNewsComponent,
   TrustedPartnerComponent,
   CtaImage,
   FooterComponent,
  },
  data(){
    return{
      navMenu: [
        {
          active: true,
          text: 'home',
        },
        {
          active: false,
          text: 'about',
        },
        {
          active: false,
          text: 'services',
        },
        {
          active: false,
          text: 'work',
        },
        {
          active: false,
          text: 'articles',
        },
        {
          button: true,
          active: false,
          text: 'get quote',
        }
      ],
      footerMenu: [
        {
          image: '../assets/img/footer-logo.png',
        },
        {
          text: 'about',
        },
        {
          active: false,
          text: 'services',
        },
        {
          active: false,
          text: 'work',
        },
        {
          active: false,
          text: 'articles',
        },
        {
          button: true,
          active: false,
          text: 'get quote',
        }
      ]
    }
  }
}
</script>

<style lang="scss">
  @import "@/style/common.scss";
</style>
