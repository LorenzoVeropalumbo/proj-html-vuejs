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

}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";
  
  section{
    margin-bottom: 40px;
    position: relative;
    .img{      
      background-image: url("../assets/img/home-244125289.jpg");
      background-repeat: no-repeat;  
      background-position: center;
      background-size: 100%;
      
      height: 1000px;

      .standard-wave{
        position: absolute;
        bottom: 0px;
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
        color: #fed03d;

        i{
          font-size: 90px;
        }

        h6{
          font-size: 80px;
          padding: 10px 0;
          font-weight: 500;
        }

        span{
          font-family: 'Montserrat', sans-serif;
          color: white;
          font-size: 20px;
          text-transform: uppercase;
          font-weight: 500;
        }
      }
    }
  }
  
</style>