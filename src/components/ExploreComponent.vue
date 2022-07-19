<template>
  <section>
    <div>
      <span class="section-title">{{ExploreWork.title}}</span>
      <div class="line"></div>
      <p class="section-subtitle">
        {{ExploreWork.subTitle}}
      </p>
    </div>

    <div class="image-container">
      <div class="overlay-cont" v-for="(image,index) in ExploreWork.images" :key="index">
        <div class="space" v-if="index < imageToShow">
          <img :src="image" alt="">
          <div class="overlay">
            <div class="text-overlay">
              <a href="#"><i class="fa-solid fa-link dot"></i></a>
              <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
              <div><span>Florida Health Facility</span></div>
              <div class="overlay-subtext"><span>Commercial</span></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="divider" v-if="!loader">
      <div class="line"></div>
      <span @click.prevent="showArticles()"><a href="#">view all articles</a></span>
      <div class="line"></div>
    </div>
    <div class="divider" v-if="loader">
      <div class="line"></div>
      <span @click.prevent="hideArticles()"><a href="#">hide articles</a></span>
      <div class="line"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ExploreComponent",
  props:{
    ExploreWork: Object,
  },
  data(){
    return{
      loader: false,
      imageToShow: 3,
    }
  },
  methods:{
    showArticles(){
      this.loader = true;
      this.imageToShow = this.ExploreWork.images.length;
    },
    hideArticles(){
      this.loader = false;
      this.imageToShow = 3;
    }
  }
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;
    text-align: center;
    padding-bottom: 30px;
    
    .image-container{
      width: 70%;
      margin: 0 auto;
      padding: 30px 20px 0;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 2rem;

      .overlay-cont{
        width: calc((100% / 3) - 2rem);    
      }
    }

    .divider{
      padding: 2rem 0 5rem;
      .line{
        background-color: $bg-button-light-grey;
      }
    }
  }
</style>