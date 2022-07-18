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
            <li v-for="(voice,index) in navMenu" :key="index" @click.prevent="setActiveElement(index)">
              <a href="#" :class="{ active : index === currentActiveElement, button : voice.button }" >{{ voice.text }}</a>
              <i class="fa-solid fa-caret-down" v-if="index === currentActiveElement"></i>
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
  },
  data(){
    return{
      currentActiveElement: 0,
    }
  },
  methods:{
    setActiveElement(index){
      if(index === 5){
        this.currentActiveElement = null;
        return null;
      }

      if(index !== this.currentActiveElement){
        this.currentActiveElement = index;
      }
    }
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
          line-height: 120px;
          position: relative;

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

          i{
            position: absolute;
            z-index: 10;
            font-size: 1.7rem;
            left: 50%;
            top: 100%;
            transform: translate(-50%,-45%);
            color: $text-white;
          }
        }
      }
    }
  }
</style>