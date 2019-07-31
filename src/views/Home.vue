<template>
  <div class="home">
    <HomeDetails class="homeDetails" />
  </div>
</template>

<script>
import HomeDetails from "@/components/HomeDetails.vue";
import main from "../assets/css/main.scss";
export default {
  name: "home",
  components: {
    HomeDetails
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