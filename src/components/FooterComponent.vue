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
          <img style="width: 70%;" src="../assets\img\Google Maps - Opera 17_07_2022 17_14_32.png" alt="">
        </div>
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

</style>