<template>
  <div id="app">
    <HeaderComponent :navMenu="navMenu" />
    <MainComponent />
    <FooterComponent />
  </div>
</template>

<script>

import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  name: 'App',
  components: {
   HeaderComponent, 
   MainComponent,
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
    }
  }
}
</script>

<style lang="scss">
  @import "@/style/common.scss";
</style>
