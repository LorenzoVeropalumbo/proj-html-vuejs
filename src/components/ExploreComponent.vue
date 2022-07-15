<template>
  <section>
    <div>
      <span class="section-title">Explore Recent Work</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.
      </p>
    </div>

    <div class="image-container">
      <div><img src="../assets/img/project2-featured-15013609.jpg" alt=""></div>
      <div><img src="../assets/img/project1-featured-294276386.jpg" alt=""></div>
      <div><img src="../assets/img/project3-featured-189023420.jpg" alt=""></div>
    </div>

    <div class="divider">
      <div class="line"></div>
      <span>view all project</span>
      <div class="line"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ExploreComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;
    text-align: center;
    padding-bottom: 30px;
    
    .section-title{
      font-size: 40px;
      color: $text-main-color;
    }

    .section-subtitle{
      width: 45%;
      margin: 0 auto;
      font-size: 18px;
      font-weight: 600;
      line-height: 45px;
      color: $text-light-grey;
    }

    .image-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      div{
        margin: 0 20px;
        width: 20%;
      }
    }

    .divider{
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 8rem 0;
      
      .line{
        margin: 0 10rem;
        width: 480px;
        background-color: $bg-button-light-grey;
      }

      span{
        text-transform: uppercase;
        letter-spacing: 2px;
        font-size: 18px;
      }
    }
  }
</style>