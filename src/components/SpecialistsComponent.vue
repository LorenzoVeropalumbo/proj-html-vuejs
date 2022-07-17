<template>
  <section>
    <div>
      <span class="section-title">Specialists In Modern Construction</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
      </p>
    </div>
    <div class="schedule-container">
      <div class="schedule">
        <div class="overlay-cont">      
          <span class="round" ><i class="fa-solid fa-building schedule-img"></i></span>
          <div>
            <span>Buildings</span>
            <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
          </div>
          <div class="overlay">
            <div class="text-overlay">
              <div><span class="title">How We Manage Large Construction Project</span></div>
              <div><span class="title">Architecture, Buildings, Construction, News</span></div>
            </div>
          </div>
        </div> 
      </div>
      <div class="schedule">
        <span class="round" ><i class="fa-solid fa-arrows-rotate"></i></span>
        <div>
          <span>Renovate</span>
          <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
        </div>
      </div>
      <div class="schedule">
        <span class="round" ><i class="fa-solid fa-house-chimney"></i></span>
        <div>
          <span>Construct</span>
          <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
        </div>
      </div>
      <div class="schedule">
        <span class="round" ><i class="fa-solid fa-truck"></i></span>
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

    .schedule-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      .schedule{
        width: 20%;
        background-color: $bg-button-light-grey;
        margin: 10px;
        border-radius: 15px;

        .round {
          height: 70px;
          width: 70px;
          line-height: 70px;
          border-radius: 50%;
          border: 2px solid #bbb;
          display: inline-block;
          font-size: 25px;
          margin: 20px 0;
        }
        
        .text-overlay{
          width: 95%;
          
          .title{
            font-size: 16px;
          }
        }
       

        span{
          font-size: 32px;
        }
        
        p{
          padding: 20px  15px 30px;
          font-size: 16px;
          line-height: 30px;
        }     
      }
    }
  }
</style>