<template>
  <section>
    <div class="img">
      <div class="flex-footer">
        <div class="col-text">
          <span class="section-title">building inspiring spaces</span>
          <div class="line"></div>
          <p class="section-subtitle">
            Vivamus sed consectetur tellus dolor sit amet, consectetur adipiscing loren elit sadip ipsum ets ficilis uns.
          </p>
        </div>
        <div class="col-btn">
          <div>
            <a href="#" class="button yellow-btn">get a free quote</a>
            <span>Only takes a few seconds!</span> 
          </div>               
        </div>
      </div>
    </div>
    <div id="separe-footer">

    </div>
    
  </section>
</template>

<script>
export default {
  name:"CtaImage",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    color: #fff;
    position: relative;

    .img{      
      background-image: url("../assets/img/about-call-to-action-57862405.jpg");
      // background-repeat: no-repeat;  
      background-position: bottom -170px right -130px;
      // background-size: 100%;
      width: 100%;
      padding-block: 140px;
      
      .flex-footer{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;

        .col-text{
          width: 35%;
          
          .section-title{
            color: $text-white;
            font-size: 28px;
            text-transform: capitalize;
          }

          .section-subtitle{
            width: 100%;
            color: #dcdbda;
            line-height: 25px;
            font-size: 18px;
            font-weight: 500;
          }

          .line{
            margin: 1.6rem 0;
          }
        }

        .col-btn{
          width: 30%;
          display: flex;
          justify-content: center;
            
          .yellow-btn{
            padding: 1rem 2rem;   
          }
          
          span{
            display: block;
            margin-block: 1.6rem;
            text-align: center;
            font-size: 12px;
          }
        }       
      }
    }

    #separe-footer{
      width: 100%;
      height: 10px;
      background-color: $text-main-color;
    }
  }
  
</style>