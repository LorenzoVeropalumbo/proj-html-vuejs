<template>
  <section>
    <div>
      <span class="section-title">Latest News</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.
      </p>
    </div>

    <div class="section-container">
      <div class="single-section">
        <div class="overlay-cont">
          <img src="../assets\img\blog-post-134132600-800x482.jpg" alt="">
          <div class="overlay">
            <div class="text-overlay">
              <a href="#"><i class="fa-solid fa-link dot"></i></a>
              <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
              <div><span>Redeveloping Florda's Remore Southern Coast</span></div>
              <div class="overlay-subtext"><span>Architecture, Buildings, Construction, News</span></div>
            </div>
          </div>
        </div>  
        <div class="section-text">
          <span class="section-title">Redeveloping Florda's Remore Southern Coast</span>
          <span class="date">December 7th, 2015</span>
          <div class="line"></div>
          <p class="paragraph">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
        </div>
      </div>
      <div class="single-section">
        <div class="overlay-cont">      
          <img src="../assets\img\blog-post-92486644-800x482.jpg" alt="">
          <div class="overlay">
            <div class="text-overlay">
              <a href="#"><i class="fa-solid fa-link dot"></i></a>
              <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
              <div><span>How We Manage Large Construction Project</span></div>
              <div class="overlay-subtext"><span>Architecture, Buildings, Construction, News</span></div>
            </div>
          </div>
        </div>       
        <div class="section-text">
          <span class="section-title">How We Manage Large Construction Project</span>
          <span class="date">December 7th, 2015</span>
          <div class="line"></div>
          <p class="paragraph">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
        </div>
      </div>
      <div class="single-section">
        <div class="overlay-cont">      
          <img src="../assets\img\blog-post-332773904-800x482.jpg" alt="">
          <div class="overlay">
            <div class="text-overlay">
              <a href="#"><i class="fa-solid fa-link dot"></i></a>
              <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
              <div><span>How We Manage Large Construction Project</span></div>
              <div class="overlay-subtext"><span>Architecture, Buildings, Construction, News</span></div>
            </div>
          </div>
        </div> 
        <div class="section-text">
          <span class="section-title">Future proofing a modern home</span>
          <span class="date">December 6th, 2015</span>
          <div class="line"></div>
          <p class="paragraph">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
        </div>
        
      </div>
    </div>

    <div class="divider" v-if="!loader">
      <div class="line"></div>
      <span @click.prevent="createLoader()"><a href="#">view all articles</a></span>
      <div class="line"></div>
    </div>
    <div class="divider" v-if="loader"><div class="loader"></div></div>
  </section>
</template>

<script>

export default {
  name: "LatestNewsComponent",
  data(){
    return{
      loader: false,
    }
  },
  methods:{
    createLoader(){
      this.loader = true;
    }
  }
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;
    text-align: center;
    background-color: $bg-button-light-grey;
    font-family: 'Raleway', sans-serif;

    .section-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      .single-section{
        margin: 0 20px;
        width: 20%;
        
        .section-text{
          padding: 40px 20px;
          background-color: $main-bg-color;
          text-align: left;
          height: 63%;

          .section-title{
            font-size: 24px;
            line-height: 35px;
          }

          .date{
            font-size: 10px;
            display: block;
            padding-top: 5px;
            font-weight: 600;
          }

          .line{
            width: 100%;
            background-color: #efeeee;
            margin: 1.6rem auto 1.6rem;
          }

          .paragraph{
            line-height: 40px;
            font-size: 16px;
          }
        }
      }
    }
    .divider{    
      .line{
        background-color: $main-bg-color;
      }
    }
  }
</style>