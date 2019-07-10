<template>
  <div class="about-details">
    <AboutDetails class="AboutDetails" />
    <MorphingArea class="MorphingArea" />
    <!-- <ButterFly class="butterfly"/> -->
  </div>
</template>

<script>
import AboutDetails from "@/components/AboutDetails.vue";
import MorphingArea from "@/components/MorphingArea.vue";
import main from "../assets/css/main.scss";
export default {
  name: "about",
  components: {
    AboutDetails,
    MorphingArea
    
  }
};
</script>

<style scoped lang="scss">


.about-details {
  grid-column: 2 / 5;
  grid-row: 2 / 4;  
 
}

.MorphingArea {
 position: relative;
 top: -900px;
}
</style>