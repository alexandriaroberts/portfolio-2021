<template>
  <div class="home">
    <HelloWorld class="helloworld" />
    <MorphingArea class="MorphingArea" />
    <!-- <ButterFly class="butterfly"/> -->
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import MorphingArea from "@/components/MorphingArea.vue";
import ButterFly from "@/components/ButterFly.vue";

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
  font-family: Lora;
  color: #000;
  background: var(--main-bg-color);
}

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