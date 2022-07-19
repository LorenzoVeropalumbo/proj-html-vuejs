<template>
  <main>
    <SpecialistsComponent />
    <PanoramaImage />
    <ExploreComponent :ExploreWork="ExploreWork" />
    <OurCoreComponent />
    <SliderComponent />
    <LatestNewsComponent />
    <TrustedPartnerComponent />
    <CtaImage />
  </main>
</template>

<script>

import SpecialistsComponent from "./SpecialistsComponent.vue";
import PanoramaImage from "./PanoramaImage.vue";
import ExploreComponent from "./ExploreComponent.vue";
import OurCoreComponent from "./OurCoreComponent.vue";
import SliderComponent from "./SliderComponent.vue";
import LatestNewsComponent from "./LatestNewsComponent.vue";
import TrustedPartnerComponent from "./TrustedPartnerComponent.vue";
import CtaImage from "./CtaImage.vue";

export default {
  name:"MainComponent",
  
  components:{
    SpecialistsComponent,
    PanoramaImage,
    ExploreComponent,
    OurCoreComponent,
    SliderComponent,
    LatestNewsComponent,
    TrustedPartnerComponent,
    CtaImage,
  },
  data(){
    return{
      ExploreWork: {
        title:"Explore Recent Work",
        subTitle: "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.",
        images:[
          require("../assets/img/project2-featured-15013609.jpg"),
          require("../assets/img/project1-featured-294276386.jpg"),
          require("../assets/img/project3-featured-189023420.jpg"),
          require("../assets/img/project2-featured-15013609.jpg"),
          require("../assets/img/project1-featured-294276386.jpg"),
          require("../assets/img/project3-featured-189023420.jpg"),
          require("../assets/img/project2-featured-15013609.jpg"),
          require("../assets/img/project1-featured-294276386.jpg"),
          require("../assets/img/project3-featured-189023420.jpg")
        ]
      }
    }
  }
}

</script>

<style lang="scss" scoped>

</style>