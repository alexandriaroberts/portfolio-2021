<template>
  <div class="home">
    <HelloWorld class="helloworld" />
    <MorphingArea class="MorphingArea" /> 
    <!-- <ButterFly/> -->
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import MorphingArea from "../components/MorphingArea";
import ButterFly from "@/components/ButterFly.vue";
import main from "../assets/css/main.scss";
export default {
  name: "home",
  components: {
    HelloWorld,
    MorphingArea,
    ButterFly
  }
};
</script>

<style scoped lang="scss">


.home {
  display: grid;
  grid-column: 2 / 5;
  grid-row: 2 / 4;
  grid-template-columns: subgrid;
  grid-template-rows: repeat(3, 1fr);
}

.MorphingArea {
  position: relative;
  grid-column: 2;
  grid-row: 1 / 4;
}
</style>