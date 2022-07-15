<template>
  <section>
    <div>
      <span class="section-title">Specialists In Modern Construction</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.
      </p>
    </div>
    <div class="schedule-container">
      <div class="schedule">
        <span class="dot" ><i class="fa-solid fa-building schedule-img"></i></span>
        <div>
          <span>Buildings</span>
          <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
        </div>
      </div>
      <div class="schedule">
        <span class="dot" ><i class="fa-solid fa-arrows-rotate"></i></span>
        <div>
          <span>Renovate</span>
          <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
        </div>
      </div>
      <div class="schedule">
        <span class="dot" ><i class="fa-solid fa-house-chimney"></i></span>
        <div>
          <span>Construct</span>
          <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
        </div>
      </div>
      <div class="schedule">
        <span class="dot" ><i class="fa-solid fa-truck"></i></span>
        <div>
          <span>Excluisive</span>
          <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SpecialistsComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    padding: 220px 0 0px;
    position: relative;
    text-align: center;
    
    
    .section-title{
      font-size: 40px;
      color: $text-main-color;
    }

    .line{
      height: 2px;
      width: 260px;
      background-color: $bg-button-yellow;
      margin: 2rem auto 2.8rem;
    }

    .section-subtitle{
      width: 55%;
      margin: 0 auto;
      font-size: 22px;
      font-weight: 600;
      line-height: 55px;
      color: #bcbcbc;
    }

    .schedule-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      .schedule{
        width: 20%;
        background-color: #f5f5f5;
        margin: 10px;
        border-radius: 15px;

        .dot {
          height: 70px;
          width: 70px;
          line-height: 72px;
          border-radius: 50%;
          border: 2px solid #bbb;
          display: inline-block;
          font-size: 25px;
          margin: 20px 0;
        }

        span{
          font-size: 42px;
        }
        
        p{
          padding: 20px  0 30px;
          font-size: 18px;
          line-height: 36px;
        }     
      }
    }
  }
</style>