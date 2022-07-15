<template>
  <div id="app">
    <HeaderComponent :navMenu="navMenu" />

    <main>
      <SpecialistsComponent />
    </main>
  </div>
</template>

<script>

import HeaderComponent from "./components/HeaderComponent.vue";
import SpecialistsComponent from "./components/SpecialistsComponent.vue";

export default {
  name: 'App',
  components: {
   HeaderComponent,
   SpecialistsComponent,
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
      ]
    }
  }
}
</script>

<style lang="scss">
  @import "@/style/common.scss";
</style>
