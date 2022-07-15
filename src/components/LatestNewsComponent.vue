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
        <img src="../assets\img\blog-post-134132600-800x482.jpg" alt="">
        <div class="section-text">
          <span class="section-title">Redeveloping Florda's Remore Southern Coast</span>
          <span class="date">December 7th, 2015</span>
          <div class="line"></div>
          <p class="paragraph">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
        </div>
      </div>
      <div class="single-section">
        <img src="../assets\img\blog-post-92486644-800x482.jpg" alt="">
        <div class="section-text">
          <span class="section-title">How We Manage Large Construction Project</span>
          <span class="date">December 7th, 2015</span>
          <div class="line"></div>
          <p class="paragraph">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
        </div>
      </div>
      <div class="single-section">
        <img src="../assets\img\blog-post-332773904-800x482.jpg" alt="">
        <div class="section-text">
          <span class="section-title">Future proofing a modern home</span>
          <span class="date">December 6th, 2015</span>
          <div class="line"></div>
          <p class="paragraph">Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed</p>
        </div>
      </div>
    </div>

    <div class="divider">
      <div class="line"></div>
      <span>view all articles</span>
      <div class="line"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "LatestNewsComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;
    text-align: center;
    background-color: $bg-button-light-grey;
    
    .section-title{
      font-family: 'Raleway', sans-serif;
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

          .section-title{
            font-size: 30px;
            line-height: 45px;
          }

          .date{
            font-size: 15px;
            display: block;
            padding-top: 15px;
          }

          .line{
            width: 100%;
            background-color: #efeeee;
            margin: 1.6rem auto 1.6rem;
          }

          .paragraph{
            line-height: 40px;
            font-size: 18px;
          }
        }
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
        background-color: $main-bg-color;
      }

      span{
        text-transform: uppercase;
        letter-spacing: 2px;
        font-size: 18px;
      }
    }
  }
</style>