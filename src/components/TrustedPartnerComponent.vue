<template>
  <section>
    <div>
      <span class="section-title">Trusted Partners</span>
      <div class="line"></div>
      <p class="section-subtitle">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.
      </p>
    </div>

    <div class="image-container">
      <div><img src="../assets/img/home-logo11-219096700-320x202.png" alt=""></div>
      <div><img src="../assets/img/home-logo10-219096700-320x202.png" alt=""></div>
      <div><img src="../assets/img/home-logo2-219096700-320x202.png" alt=""></div>
      <div><img src="../assets/img/home-logo1-219096700-320x202.png" alt=""></div>
      <div><img src="../assets/img/home-logo9-219096700-320x202.png" alt=""></div>     
    </div>
  </section>
</template>

<script>
export default {
  name: "TrustedPartnerComponent",
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";

  section{
    text-align: center;
    padding: 80px 0;

    .image-container{
      padding: 70px 20px 0;
      display: flex;
      justify-content: center;

      div{
        margin: 0 20px;
        width: 10%;
      }
    }
  }
</style>