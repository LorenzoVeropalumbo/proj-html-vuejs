<template>
  <div class="header-bottom">
    <div class="jumbtron">
      <!-- Insection Right -->
      <div class="insection-right">
        <div>
          <i class="fa-solid fa-images"></i>
          <span class="text-bot">Demos</span>
        </div>
        <div>
          <span class="green"><span class="green pos-top">$</span>39</span>
          <span class="text-bot">On Sale</span>
        </div>
      </div>

      <!-- Text Jumbotron -->
      <div class="text-center">
        <div>
          <div id="big-text"><span>Building inspiring spaces</span></div>
          <div class="alternative-text"><span>We Build Inspiring Residential & Commercial Spaces</span></div>
          <div class="button-container">
            <a href="#" class="button grey-btn">explore recent work</a>
            <a href="#" class="button yellow-btn">get a quote today</a>
          </div> 
        </div> 
      </div>
    </div>
    <!-- Button banner yellow -->
    <div class="cta">
      <div class="text-center">
        <span class="alternative-text">Do You Have A Construction Project We Can Help With?</span>
      </div>

      <div class="btn-relative-pos">
        <a href="#" class="button grey-btn">Get a free quote</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderJumboCta",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  .header-bottom{
    
    .jumbtron{
      height: calc(100vh - 120px);
      width: 100%;
      background-image: url("../assets/img/home-slider-62528242.jpg");
      background-position: top;
      background-repeat: no-repeat;
      background-size: cover;
      position: relative;

      .insection-right{
        position: absolute;
        top: 20px;
        right: 20px;   
        font-family: Arial, Helvetica, sans-serif;  

        div{
          background-color: $main-bg-color;
          border-radius: 10px;
          margin: 8px;
          height: 80px;
          width: 80px;
          padding: 10px 0;

          i{
            font-size: 30px;
            padding: 5px 25px 3px;
            color: #33475b;
          }

          > .green{
            font-size: 35px;
            color: #66bc7b;
            font-weight: 700;
            display: block;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            padding-left: 5px;
            padding-bottom: 3px;
            
            .pos-top{
              position: absolute;
              left: 15%;
              top: 5%;
              font-size: 20px;
            }
          }

          .text-bot{
            display: block;
            text-align: center;
            font-weight: 700;
          }
        }
      }

      .text-center{
        color: $text-white;

        #big-text{
          font-size: 55px;
          text-transform: uppercase;
          font-weight: 600;
        }

        .alternative-text{
          padding-block: 30px;
          font-size: 24px;
          color: $text-subtitle;
        }
        
        .button-container{
          padding-top: 50px;
          font-size: 16px;

          .button{
            padding: 1.3rem 2.7rem;
            margin: 0.9rem;
          }
        }      
      }      
    }
    
    .cta{
      padding: 75px 0;
      background-color: $cta-bg-color;
      position: relative;

      .alternative-text{
        font-size: 30px;
      }

      .btn-relative-pos{
        position: absolute;
        top: calc(100% - 27px);
        left: 50%;
        transform: translate(-50%, 0);
        background-color: $main-bg-color;
        padding: 15px 2px;
        z-index: 9999;
        
        .button{
          padding: 0.8rem 2rem;    
        }

        &:hover{
          background: black;

          .grey-btn{
            background-color: $main-bg-color;
            color: black;
          }
        }
      }
    }
  }
</style>