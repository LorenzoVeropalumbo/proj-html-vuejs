<template>
  <header>
    <!-- HEADER TOP -->
    <div class="header-top">
      <!-- MENU TOP CONTAINER -->
      <div class="header-top-container">
        <img src="../assets/img/construction_logo.png" alt="construction_logo">
        <nav>
          <ul class="ul-nav-menu">
            <!-- MENU LIST ITEM -->
            <li v-for="(voice,index) in navMenu" :key="index" @click.prevent="setActiveElement(index)">
              <a href="#" :class="{ active : index === currentActiveElement, button : voice.button }">{{ voice.text }}</a>
              <i class="fa-solid fa-caret-down" v-if="index === currentActiveElement"></i>
              <ul class="dropdown-menu" v-if="index === currentActiveElement">
                <li v-for="(listItem,index) in voice.liDynamic" :key="index">
                  <span><i class="fa-solid fa-angle-right"></i></span>
                  <a :href="listItem.href">{{listItem.text}}</a>
                </li>
              </ul>
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
      currentActiveElement: null,
    }
  },
  methods:{
    setActiveElement(index){
      
      if (index === 5) {
        this.currentActiveElement = null;
        return null;
      } else if (index !== this.currentActiveElement) {
        this.currentActiveElement = index;
      } else {
        this.currentActiveElement = null;
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

      .ul-nav-menu{
        display: flex;
        align-items: center;
        text-transform: uppercase;
        font-size: 14px;
        position: relative;
        z-index: 99;       

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

          .dropdown-menu{
            position: absolute;
            z-index: 1;
            font-size: 0.8rem;
            left: 50%;
            top: 100%;
            transform: translate(-50%, 0%);
            color: $text-white;
            background-color: rgba(128, 128, 128, 0.2);
            padding-top: 0.6rem;

            li{
              padding-block: 0.7rem;
              padding-inline: 1rem 3rem;
              line-height: 1rem;
              display: block;

              i{
                font-size: 0.8rem;
                display: inline;
                position: initial;
                padding-right: 0.6rem;
              }

              &:hover *{
                color: $active-text;
              }
            }
          }
        }
      }
    }
  }
</style>