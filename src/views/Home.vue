<template>
  <div class="home">
    <HomeDetails class="homeDetails" />
    <!-- <MorphingArea class="MorphingArea" />  -->
    <!-- <ButterFly/> -->
  </div>
</template>

<script>
import HomeDetails from "@/components/HomeDetails.vue";
import MorphingArea from "../components/MorphingArea";
import ButterFly from "@/components/ButterFly.vue";
import main from "../assets/css/main.scss";
export default {
  name: "home",
  components: {
    HomeDetails,
    MorphingArea,
    ButterFly
  }
};
</script>

<style scoped lang="scss">
.home {
  grid-column: 2 / 4;
  grid-row: 2 / 5;
  padding-top: 1em;
}

@media (max-width: 760px) {
  .home {
    grid-column: 1 / 5;
    padding-top: 1.5rem;
  }
}
</style>