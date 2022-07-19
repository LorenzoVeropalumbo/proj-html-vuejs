<template>
  <div id="app">
    <HeaderComponent :navMenu="navMenu" />
    <MainComponent />
    <FooterComponent :footerMenu="footerMenu"/>
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
          liDynamic:[
            {
              text: 'info',
              href: "#",
            }
          ]
        },
        {
          active: false,
          text: 'about',
          liDynamic:[
            {
              text: 'Contact',
              href: "#",
            },
            {
              text: 'About',
              href: "#",
            }
          ]
        },
        {
          active: false,
          text: 'services',
          liDynamic:[
            {
              text: 'Quotes',
              href: "#",
            },
            {
              text: 'Info',
              href: "#",
            }
          ]
        },
        {
          active: false,
          text: 'work',
          liDynamic:[
            {
              text: 'Work',
              href: "#",
            },
            {
              text: 'Parnets',
              href: "#",
            }
          ]
        },
        {
          active: false,
          text: 'articles',
          liDynamic:[
            {
              text: 'Review',
              href: "#slider-component",
            },
          ]
        },
        {
          button: true,
          active: false,
          text: 'get quote',
        }
      ],
      footerMenu: [
        {
          icon:"fa-solid fa-globe",
          texts: ["Corporate Location","1600 Amphitheatre Parkway","London WC1 1BA"]
        },
        {
          icon:"fa-solid fa-house-chimney",
          texts: ["Residential Location","9521 broadsberry Avenue","Paddington RC7 9ZA"]
        },
        {
          icon:"fa-solid fa-phone-flip",
          texts: ["1.800.458.556 / 1.800.532.2112"]
        },
        {
          icon:"fa-regular fa-envelope",
          texts: ["info@your-domain.com"]
        },
        {
          icon:"fa-regular fa-clock",
          texts: ["Monday - Friday: 9:00 AM - 6:00 PM"]
        },
        {
          icon:"fa-regular fa-clock",
          texts: ["Saturday - Sunday: 9:00 AM - 12:00 PM"]
        },
      ],
    }
  }
}
</script>

<style lang="scss">
  @import "@/style/common.scss";
</style>
