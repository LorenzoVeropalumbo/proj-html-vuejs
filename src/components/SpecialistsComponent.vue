<template>
  <section>
    <div>
      <!-- Titles -->
      <span class="section-title">Specialists In Modern Construction</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
      </p>
    </div>
    <!-- Container -->
    <div class="schedule-container">
      <div class="schedule">
        <div class="overlay-cont">      
          <span class="round" ><i class="fa-solid fa-building"></i></span>
          <div>
            <!-- card text -->
            <span>Buildings</span>
            <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
          </div>
          <!-- overlay effect -->
          <div class="overlay">
            <div class="text-overlay">
              <span class="title">ARTFULLY CRAFTED</span>
              <span class="sub-title">Quis autem vel eum irue reprederit qui in ea voluptate velit esse quam nihil molistiae consequatur, vel illum qui dolorem eum.</span>
              <div><a href="#" class="button yellow-btn">GET A QUOTE</a></div>
            </div>
          </div>
        </div> 
      </div>
      <div class="schedule">
        <div class="overlay-cont">      
          <span class="round" ><i class="fa-solid fa-arrows-rotate"></i></span>
          <div>
            <!-- card text -->
            <span>Renovate</span>
            <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
          </div>
          <!-- overlay effect -->
          <div class="overlay">
            <div class="text-overlay">
              <span class="title">ARTFULLY CRAFTED</span>
              <span class="sub-title">Quis autem vel eum irue reprederit qui in ea voluptate velit esse quam nihil molistiae consequatur, vel illum qui dolorem eum.</span>
              <div><a href="#" class="button yellow-btn">GET A QUOTE</a></div>
            </div>
          </div>
        </div>          
      </div>
      <div class="schedule">
        <div class="overlay-cont">      
          <span class="round" ><i class="fa-solid fa-house-chimney"></i></span>
          <div>
            <!-- card text -->
            <span>Construct</span>
            <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
          </div>
          <!-- overlay effect -->
          <div class="overlay">
            <div class="text-overlay">
              <span class="title">ARTFULLY CRAFTED</span>
              <span class="sub-title">Quis autem vel eum irue reprederit qui in ea voluptate velit esse quam nihil molistiae consequatur, vel illum qui dolorem eum.</span>
              <div><a href="#" class="button yellow-btn">GET A QUOTE</a></div>
            </div>
          </div>
        </div>
      </div>
      <div class="schedule">
        <div class="overlay-cont">      
          <span class="round"><i class="fa-solid fa-truck"></i></span>
          <div>
            <!-- card text -->
            <span>Excluisive</span>
            <p>Quis autem vel eum lure reprederit qui in ea voluptate velit esse quam nikil molestiae consequatur. </p>
          </div>
          <!-- overlay effect -->
          <div class="overlay">
            <div class="text-overlay">
              <span class="title">ARTFULLY CRAFTED</span>
              <span class="sub-title">Quis autem vel eum irue reprederit qui in ea voluptate velit esse quam nihil molistiae consequatur, vel illum qui dolorem eum.</span>
              <div><a href="#" class="button yellow-btn">GET A QUOTE</a></div>
            </div>
          </div>
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

        .overlay{
          border-radius: 20px;
        }
        
        .text-overlay{
          width: 95%;
          color: black;
          
          .title{
            display: block;
            font-size: 18px;
          }

          .sub-title{
            display: block;
            font-size: 14px;
            line-height: 28px;
            margin-block: 20px 30px;
          }

          a{
            font-size: 16px;
            letter-spacing: 2px;
          }

          .button{
            padding: 0.7rem 1.4rem;

          }

          .yellow-btn{
            background-color: #ffe07b;

            &:hover{
              background-color: black;
            }
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