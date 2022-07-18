<template>
  <section>
    <div class="img">
      <img class="standard-wave" src="../assets/img/wave2.svg" alt="nomal-wave">
      <img :src="slides[currentActiveElement].image" :alt="slides[currentActiveElement].alt">
      <img class="rotate-wave" src="../assets/img/wave2.svg" alt="nomal-wave">
    </div>

    <div class="text-center">
      <div class="info">
        <span class="section-title">Our Home Owners Say</span>
        <div class="line"></div>
        <img :src="slides[currentActiveElement].imageTestimonial" :alt="slides[currentActiveElement].alt">
        <p class="section-subtitle">
          &#34; {{ slides[currentActiveElement].testimonialText }} &#34;
        </p>
        <span class="review-name">{{ slides[currentActiveElement].testimonialName }} <span class="small-circle">&#9679;</span> new home owner </span>
        <ul class="silder-circle">
          <li v-for="(slide,index) in slides" :key="index"  @click="clickSlides(index)" class="thumb" :class="{'active': index === currentActiveElement}">
          </li>
        </ul>
      </div>   
    </div>
  </section>
</template>

<script>
export default {
  name:"SliderComponent",
  data(){
    return{
      currentActiveElement: 0,

      slides: [
        {
          image: require('../assets/img/home-parallax-144609983.jpg'),
          imageTestimonial: require("../assets/img/home-testimonial-113165296.jpg"),
          testimonialName: "Clara smith",
          testimonialText: "No man but feels more of a man in the world if he have but a bit ok ground that he can call his own. However small it is on the surface, it is four thousand miles deep; and that is a very handsome property.",
          alt: "home"
        },
        {
          image: require('../assets/img/r-architecture-2gDwlIim3Uw-unsplash-uai-2560x1920.jpg'),
          imageTestimonial: require( "../assets/img/home-testimonial-84268399.jpg"),
          testimonialName: "Harry Potter",
          testimonialText: "Se la vita ti da limoni, fatti una limonata",
          alt: "home"
        },
      ]
    }
  },
  methods:{
    clickSlides(index){
      this.currentActiveElement = index;
    }
  }
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;

    .img{      
      height: 1000px;

      .standard-wave{
        position: absolute;
        bottom: -5px;
        right: 0px;
      }

      .rotate-wave{
        position: absolute;
        top: -5px;
        right: 0px;
        transform: rotate(180deg);
      }
    }

    .text-center{
      display: flex;
      width: 45%; 
      justify-content: center;
      align-items: center;
      font-family: 'Raleway', sans-serif;
      

      .info{
        font-family: 'Raleway', sans-serif;
        color: $text-white;

        .section-title{
          font-size: 35px;
          color: $text-white;
        }

        img{
          margin: 0 auto;
          vertical-align: middle;
          width: 160px;
          border-radius: 450px;
        }

        .section-subtitle{
          width: 88%;
          font-family: 'Raleway', sans-serif;
          font-style: italic;
          padding: 38px 0;
          letter-spacing: 2px;
          color: $text-white;
        }

        .review-name{
          font-weight: 800;
          font-size: 16px;
          text-transform: uppercase;
          letter-spacing: 2px;
          line-height: 21px;

          .small-circle{
            font-size: 10px;
            vertical-align: bottom;
            padding: 0 2px;
          }
        }

        .silder-circle{
          display: flex;
          justify-content: center;
          padding-top: 50px;

          li{
            margin-right: 10px;
            cursor: pointer;
          }

          .thumb{
            width: 15px;
            height: 15px;
            border: 1px solid $text-white;
            border-radius: 50%;

            &.active{
              background-color: $text-white;
            }
          }
        }
      }
    }
  }
  
</style>