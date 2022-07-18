<template>
  <footer>
    <div class="footer-top">
      <div class="col">
        <div class="card">
          <img class="avada-footer-logo" src="../assets/img/footer-logo.png" alt="">
          <p class="avada-text">We are specialists in the construction of unique and exclusive properties. Our work inspires. We pride ourselves on delivering outstanding quality and design for leading clients across the world.</p>
          <a href="#" class="button yellow-btn">LEARN MORE</a>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <h5>latest tweets</h5>
          <div class="tweet-section">
            <div class="profile-img"><img src="../assets\img\3a74ce3d0532b7773b174c45ca3bd05a_bigger.png" alt=""></div>
            <div class="tweet-text">
              <div class="tweetter-info">
                <div>
                  <span class="name-tweet">ThemeFusion</span>
                  <span class="account-tweet">@ThemeFusion</span>
                </div> 
                <img src="../assets\img\image (1).svg" alt="tweetter logo"> 
              </div>            
              <p>
                Do you need sublime WorldPress hosting for your next website? Take advantage of exclusive partners offers that we have secured just for you, & launch your site in second width <span class="blue">#avada</span> on WP Engine hosting & get 30% Off this Black Friday <a href="#" class="blue">
                bit.ly/3kjLLE2</a> <span class="blue">#BlackFriday2020</span>
              </p>
              <img src="../assets\img\En2TRxLW4AEiWUN.jpeg" alt="offert immage">
              <div class="link-img">
                <div>
                  <img src="../assets\img\image (2).svg" alt="heart">
                  <img src="../assets\img\image (3).svg" alt="learn more">
                </div>               
                <span>22h</span>
              </div>      
            </div>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <h5>Contact us today</h5>
          <ul class="fa-ul" style="--fa-li-margin: 1em;">
            <li><span class="fa-li"><i class="fa-solid fa-globe"></i></span><p>Corporate Location<br>1600 Amphitheatre Parkway<br>London WC1 1BA</p></li>
            <li><span class="fa-li"><i class="fa-solid fa-house-chimney"></i></span><p>Residential Location<br>9521 broadsberry Avenue<br>Paddington RC7 9ZA</p></li>
            <li><span class="fa-li"><i class="fa-solid fa-phone-flip"></i></span><p>1.800.458.556 / 1.800.532.2112</p></li>
            <li><span class="fa-li"><i class="fa-regular fa-envelope"></i></span><p>info@your-domain.com</p></li>
            <li><span class="fa-li"><i class="fa-regular fa-clock"></i></span><p>Monday - Friday: 9:00 AM - 6:00 PM</p></li>
            <li><span class="fa-li"><i class="fa-regular fa-clock"></i></span><p>Saturday - Sunday: 9:00 AM - 12:00 PM</p></li>
          </ul>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <h5>Find us</h5>
          <div class="mapouter"><div class="gmap_canvas"><iframe width="350" height="300" id="gmap_canvas" src="https://maps.google.com/maps?q=london,notting&t=&z=13&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe><a href="https://2piratebay.org"></a><br><a href="https://www.embedgooglemap.net"></a></div></div>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container-bottom">
        <div>copyright 2012 - 2015 Avada theme by <b>theme fusion</b> | all rights reserved | powered by <b>WorldPress</b></div>
        <div>
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-youtube"></i>
          <i class="fa-brands fa-instagram"></i>
        </div>
        <div class="down-arrow"><a href="#"><i class="fa-solid fa-angle-up"></i></a></div>
      </div>
    </div>
  </footer>
</template>

<script>
  
  export default {
    name:"FooterComponent",
  }
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  .footer-top{
    font-family: 'Raleway', sans-serif;
    padding: 60px 4rem;
    display: flex;
    justify-content: space-between;
    background-color: #1e1e1e;

    .col{
      width: 25%;
      padding: 0 25px;

      .avada-footer-logo{
        width: 50%;
      }

      .avada-text{
        padding-block: 2.6rem;
        line-height: 2rem;
      }

      .button{
        padding: 0.7rem 2rem;
      }

      h5{
        text-transform: uppercase;
        color: #f6c93b;
        padding-bottom: 2rem;
        font-size: 0.9rem;
      }

      .tweet-section{
        color: $text-white;
        display: flex;
        font-size: 0.8rem;

        .profile-img{
          width: 8%;
          flex-shrink: 0;
          margin-right: 10px;
          img{
            border-radius: 50%;
          }
        }

        p{
          padding-block: 3px 30px;
          .blue{
            color: #2972aa;
          }
        }

        .tweetter-info{
          display: flex;
          justify-content: space-between;
          align-items: flex-start;

          div span{
            display: block;
          }

          .name-tweet{
            font-weight: 600;
          }

          .account-tweet{
            color: #aab3b9;
          }

          img{
            width: 5%;
          }

          .mapouter{
            width: 100%;
          }
        }

        .link-img{
          display: flex;
          justify-content: space-between;
          align-items: flex-end;
          div{
            img{
              display: inline-block;
              width: 20%;
              padding-top: 10px;
              margin-right: 25px;
              cursor: pointer;
            }
          }
        
          span{
            display: inline;
            text-align: right;
            color: #4a535a;
            font-weight: 600;
          }
        }
      }

      ul{
        padding: 0 10px;
      }

      li{
        font-size: 0.9rem;
        line-height: 1.3rem;
        font-weight: 600;
        padding: 4px 4px;
      }
    }
  }

  .footer-bottom{
    background-color: #111111;
    padding-block: 1.5rem;
    font-size: 0.6rem;
    text-transform: uppercase;
    overflow: hidden;
    
    .container-bottom{
      width: 90%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      position: relative;

      i{
        padding: 0 10px;
        font-size: 1.1rem;
      }

      .down-arrow{
        position: absolute;
        color: $text-white;
        left: 98.4%;
        top: 50%;
        background-color: #303030;
        opacity: 0.8;
        border-radius: 5px;
        padding: 12px 8px;

        i{
          font-size: 0.8rem;
        }
      }
    }
  }  
</style>