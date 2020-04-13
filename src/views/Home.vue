<template>
  <div class="home">
    <Hero />
    <AboutDetails class="AboutDetails" />
    <Skills />
    <Achievements />
    <Work />
  </div>
</template>

<script>
import Hero from "@/components/Hero.vue";
import AboutDetails from "@/components/AboutDetails.vue";
import Skills from "@/components/Skills.vue";
import Achievements from "@/components/Achievements.vue";
import Work from "@/components/Work.vue";

export default {
  name: "home",
  components: {
    Hero,
    AboutDetails,
    Skills,
    Achievements,
    Work
  }
};
</script>

<style scoped lang="scss">
.home {
  grid-row: 2 / -1;
  grid-column: 1 / -1;

  // Home Page Grid Layput
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(3, min-content);
  grid-gap: 13rem 0;
}
</style>
