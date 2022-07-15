<template>
  <section>
    <div class="img">
      <img class="standard-wave" src="../assets/img/wave2.svg" alt="nomal-wave">
      <img class="rotate-wave" src="../assets/img/wave2.svg" alt="nomal-wave">
    </div>

    <div class="text-center">
      <div class="info">
        <span class="section-title">Our Home Owners Say</span>
        <div class="line"></div>
        <p class="section-subtitle">
          "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam."
        </p>
      </div>   
    </div>
  </section>
</template>

<script>
export default {
  name:"SliderComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;

    .img{      
      background-image: url("../assets/img/home-parallax-144609983.jpg");
      background-repeat: no-repeat;  
      background-position: center;
      background-size: 100%;
      width: 100%;
      height: 1200px;

      .standard-wave{
        position: absolute;
        bottom: -5px;
      }

      .rotate-wave{
        position: absolute;
        top: -5px;
        transform: rotate(180deg);
      }
    }

    .text-center{
      display: flex;
      width: 55%; 
      justify-content: center;
      align-items: center;
      font-family: 'Raleway', sans-serif;
      

      .info{
        font-family: 'Raleway', sans-serif;
        color: $text-white;

        .section-title{
          font-size: 42px;
        }

        .section-subtitle{
          font-size: 25px;
          font-family: 'Raleway', sans-serif;
          font-style: italic;
        }
      }
    }
  }
  
</style>