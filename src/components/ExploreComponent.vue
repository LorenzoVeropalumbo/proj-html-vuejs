<template>
  <section>
    <div>
      <span class="section-title">Explore Recent Work</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.
      </p>
    </div>

    <div class="image-container">
      <div class="overlay-cont">
        <img src="../assets/img/project2-featured-15013609.jpg" alt="">
        <div class="overlay">
          <div class="text-overlay">
            <a href="#"><i class="fa-solid fa-link dot"></i></a>
            <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
            <div><span>Florida Health Facility</span></div>
            <div class="overlay-subtext"><span>Commercial</span></div>
          </div>
        </div>
      </div>
      <div class="overlay-cont">
        <img src="../assets/img/project1-featured-294276386.jpg" alt="">
        <div class="overlay">
          <div class="text-overlay">
            <a href="#"><i class="fa-solid fa-link dot"></i></a>
            <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
            <div><span>Florida Health Facility</span></div>
            <div class="overlay-subtext"><span>Commercial</span></div>
          </div>
        </div>
      </div>
      <div class="overlay-cont">
        <img src="../assets/img/project3-featured-189023420.jpg" alt="">
        <div class="overlay">
          <div class="text-overlay">
            <a href="#"><i class="fa-solid fa-link dot"></i></a>
            <a href="#"><i class="fa-solid fa-magnifying-glass dot"></i></a>
            <div><span>Florida Health Facility</span></div>
            <div class="overlay-subtext"><span>Commercial</span></div>
          </div>
        </div>
      </div>
    </div>

    <div class="divider">
      <div class="line"></div>
      <span><a href="">view all project</a></span>
      <div class="line"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ExploreComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    position: relative;
    text-align: center;
    padding-bottom: 30px;

    .image-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      .overlay-cont{
        margin: 0 20px;
        width: 20%;    
      }  
    }

    .divider{    
      .line{
        background-color: $bg-button-light-grey;
      }
    }
  }
</style>