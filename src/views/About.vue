<template>
<!-- About page -->
  <div class="about-details">
    <AboutDetails class="AboutDetails" />
  </div>
</template>

<script>
import AboutDetails from "@/components/AboutDetails.vue";
import main from "../assets/css/main.scss";
export default {
  name: "about",
  components: {
    AboutDetails
     
  }
};
</script>

<style scoped lang="scss">
.about-details {
  grid-column: 2 / 4;
  grid-row: 2 / 5;  
 }


// CSS for Mobile View
@media (max-width: 960px) {
  .about-details {
  grid-column: 1 / 5;
  grid-row: 2 / 5;  
 justify-self: center;
 align-self: center;
}
}

</style>