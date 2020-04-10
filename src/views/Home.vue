<template>
  <div class="home">
    <!-- <HomeDetails class="homeDetails" /> -->
    <Hero />
     <AboutDetails class="AboutDetails" />
  </div>
</template>

<script>
import HomeDetails from '@/components/HomeDetails.vue'
import Hero from '@/components/Hero.vue'
import AboutDetails from "@/components/AboutDetails.vue";

export default {
  name: 'home',
  components: {
    Hero,
    AboutDetails
  }
}
</script>

<style scoped lang="scss">
.home {
  grid-row: 2 / -1;
  grid-column: 1 / -1;

// Home Page Grid Layput
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(3, min-content);
  grid-gap: 6.5rem 0;
}

</style>
