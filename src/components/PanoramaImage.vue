<template>
  <section>
    <div class="img">
      <img class="standard-wave" src="../assets/img/wave.svg" alt="nomal-wave">
      <img class="rotate-wave" src="../assets/img/wave.svg" alt="nomal-wave">
    </div>

    <div class="text-center">
      <div class="info">
        <i class="fa-solid fa-suitcase"></i>
        <h6>3534</h6>
        <span>planning Application</span>
      </div>
      <div class="info">
        <i class="fa-regular fa-building"></i>
        <h6>896</h6>
        <span>completed project</span>
      </div>
      <div class="info">
        <i class="fa-solid fa-users"></i>
        <h6>172</h6>
        <span>trained professionals</span>
      </div>
      <div class="info">
        <i class="fa-solid fa-globe"></i>
        <h6>19</h6>
        <span>international offices</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name:"PanoramaImage",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;

    .img{      
      background-image: url("../assets/img/home-244125289.jpg");
      background-repeat: no-repeat;  
      background-position: center;
      background-size: 100%;
      width: 100%;
      padding-block: 350px;

      .standard-wave{
        position: absolute;
        bottom: -5px;
      }

      .rotate-wave{
        position: absolute;
        top: -5px;
        transform: rotate(180deg)
      }
    }

    .text-center{
      display: flex;
      width: 55%;
      justify-content: space-between;
      align-items: center;

      .info{
        font-family: 'Raleway', sans-serif;
        color: $text-subtitle;

        i{
          font-size: 70px;
        }

        h6{
          font-size: 55px;
          padding: 0 0 10px;
          font-weight: 500;
        }

        span{
          font-family: 'Montserrat', sans-serif;
          color: $text-white;
          font-size: 16px;
          text-transform: uppercase;
          font-weight: 500;
        }
      }
    }
  }
  
</style>