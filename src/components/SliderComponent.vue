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
        <img src="../assets\img\home-testimonial-113165296.jpg" alt="testimonial 1">
        <p class="section-subtitle">
          "No man but feels more of a man in the world if he have but a bit ok ground that he can call his own. However small it is on the surface, it is four thousand miles deep; and that is a very handsome property."
        </p>
        <span class="review-name">Harry smith <span class="small-circle">&#9679;</span> new home owner </span>
        <ul class="silder-circle">
          <li class="circle-full"></li>
          <li class="circle-empty"></li>
        </ul>
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
      width: 38%; 
      justify-content: center;
      align-items: center;
      font-family: 'Raleway', sans-serif;
      

      .info{
        font-family: 'Raleway', sans-serif;
        color: $text-white;

        .section-title{
          font-size: 42px;
        }

        img{
          margin: 0 auto;
          vertical-align: middle;
          width: 180px;
          border-radius: 450px;
        }

        .section-subtitle{
          font-size: 25px;
          font-family: 'Raleway', sans-serif;
          font-style: italic;
          line-height: 40px;
          padding: 38px 0;
        }

        .review-name{
          font-weight: 800;
          font-size: 22px;
          text-transform: uppercase;

          .small-circle{
            font-size: 12px;
            line-height: 26px;
            padding: 2px 8px;
            vertical-align: text-bottom;  
          }
        }

        .silder-circle{
          display: flex;
          justify-content: center;
          padding-top: 50px;

          li{
            margin-right: 10px;
          }

          .circle-empty{
            width: 15px;
            height: 15px;
            border: 1px solid white;
            border-radius: 50%;
          }

          .circle-full{
            width: 15px;
            height: 15px;
            background-color: white;
            border-radius: 50%;
          }
        }
      }
    }
  }
  
</style>