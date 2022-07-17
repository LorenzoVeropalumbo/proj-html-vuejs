<template>
  <header>
    <!-- HEADER TOP -->
    <div class="header-top">
      <!-- MENU TOP CONTAINER -->
      <div class="header-top-container">
        <img src="../assets/img/construction_logo.png" alt="construction_logo">
        <nav>
          <ul>
            <!-- MENU LIST ITEM -->
            <li v-for="(voice,index) in navMenu" :key="index">
              <a href="#" :class="{ active : voice.active, button : voice.button }" >{{ voice.text }}</a>
            </li>
          </ul>
        </nav>
      </div>  
    </div>
    <!-- JUMBOTRON -->
    <HeaderJumboCta />
  </header>
</template>

<script>

import HeaderJumboCta from "./HeaderJumboCta.vue";

export default {
  name: "HeaderComponent",
  props:{
    navMenu: Array
  },
  components:{
    HeaderJumboCta,
  }
  
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  .header-top{
    height: 120px;
    background-color: $main-bg-color;

    .header-top-container{
      width: 94%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin: 0 auto;
      height: 100%;

      img{
        width: 200px;      
      }

      ul{
        display: flex;
        align-items: center;
        text-transform: uppercase;
        font-size: 14px;       

        li{
          padding: 0 1.8rem;

          .active{
            color: $active-text;
            font-weight: 500;
          }

          .button{
            background-color: $bg-button-yellow;
            padding: 0.9rem 2.2rem;

            &:hover{
              background-color: $bg-button-grey;
              color: $text-white;
            }
          }
        }
      }
    }
  }
</style>