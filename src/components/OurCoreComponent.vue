<template>
  <section>
    <div>
      <span class="section-title">Our Core Values</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.
      </p>
    </div>
    <div class="schedule-container">
      <div class="schedule">
        <span class="dot cyan"><i class="fa-solid fa-house-chimney"></i></span>
        <div>
          <span>Great Service</span>
          <div class="line"></div>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia</p>
        </div>
      </div>
      <div class="schedule">
        <span class="dot blue" ><i class="fa-solid fa-gear"></i></span>
        <div>
          <span>Highest Standards</span>
          <div class="line"></div>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia</p>
        </div>
      </div>
      <div class="schedule">
        <span class="dot orange" ><i class="fa-solid fa-house-chimney"></i></span>
        <div>
          <span>Professional Team</span>
          <div class="line"></div>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia</p>
        </div>
      </div>
      <div class="schedule">
        <span class="dot green" ><i class="fa-solid fa-truck"></i></span>
        <div>
          <span>Creative Solutions </span>
          <div class="line"></div>
          <p>Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "OurCoreComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    padding: 120px 0 0px;
    position: relative;
    text-align: center;
    background-color: $bg-button-light-grey;

    .schedule-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      .schedule{
        width: 18%;
        margin: 10px;
        border-radius: 15px;

        .dot {
          height: 120px;
          width: 120px;
          line-height: 120px;
          border-radius: 50%;
          display: inline-block;
          font-size: 50px;
          margin: 20px 0;
          color: $text-white;
        }

        .line{
          width: 30px;
          height: 3px;
          margin: 20px auto 10px;
          background-color: #8f8f8f;
        }

        .cyan{
          background-color: #4da4a5;
        }

        .blue{
          background-color: #4f6da5;
        }

        .orange{
          background-color: #f6722b;
        }

        .green{
          background-color: #a7cf47;
        }

        span{
          font-size: 15px;
          font-weight: 400;
        }
        
        p{
          padding-top: 10px;
          font-size: 15px;
          line-height: 36px;
          font-weight: 400;
        }     
      }
    }
  }
</style>