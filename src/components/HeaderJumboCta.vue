<template>
  <div class="header-bottom">
    <div class="jumbtron">
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
      height: 1010px;
      width: 100%;
      background-image: url("../assets/img/home-slider-62528242.jpg");
      background-position: top;
      background-repeat: bottom;
      position: relative;

      .insection-right{
        position: absolute;
        top: 20px;
        right: 20px;     

        div{
          background-color: white;
          border-radius: 10px;
          margin: 8px;
          height: 90px;
          width: 90px;
          padding: 10px 0;

          i{
            font-size: 40px;
            padding: 5px 25px 10px;
            color: #33475b;
          }

          > .green{
            font-size: 40px;
            color: #66bc7b;
            font-weight: 700;
            display: block;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            padding-left: 10px;
            padding-bottom: 5px;
            font-family: Arial, Helvetica, sans-serif;

            .pos-top{
              position: absolute;
              left: 20%;
              top: 10%;
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
          font-size: 65px;
          text-transform: uppercase;
          font-weight: 600;
        }

        .alternative-text{
          padding-block: 30px;
          font-size: 28px;
          color: $text-subtitle;
        }
        
        .button-container{
          padding-top: 50px;
          font-size: 20px;

          .yellow-btn{
            background-color: $bg-button-yellow;
            padding: 1.3rem 2.7rem;
            color: $text-main-color;
            margin: 0.9rem;
          }
          .grey-btn{
            background-color: $bg-button-grey;
            padding: 1.3rem 2.7rem;
            color: $text-white;
            margin: 0.9rem;
          }
        }
        
      }      
    }
    
    .cta{
      height: 150px;
      background-color: $cta-bg-color;
      position: relative;

      .alternative-text{
        font-size: 38px;
      }

      .btn-relative-pos{
        position: absolute;
        top: calc(100% - 13px);
        left: 50%;
        transform: translate(-50%, 0);

        .grey-btn{
          background-color: $bg-button-grey;
          padding: 0.8rem 2rem;
          color: $text-white;
          border: 3px solid white;
        }
      }
    }
  }
</style>