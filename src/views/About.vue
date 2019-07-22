<template>
<!-- About page -->
  <div class="about-details">
    <AboutDetails class="AboutDetails" />
    <!-- <MorphingArea class="MorphingArea" /> --> 
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
  grid-column: 2 / 4;
  grid-row: 2 / 5;  
 
}

.MorphingArea {
 position: relative;
 top: -900px;
}
// CSS for Mobile View
@media (max-width: 760px) {
  .about-details {
  grid-column: 1 / 5;
  grid-row: 2 / 5;  
 justify-self: center;
 align-self: center;
}
}
</style>