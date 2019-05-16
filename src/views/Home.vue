<template>
  <div class="home" id="grid-container">
    <HelloWorld class="helloworld"/>
    <FlowerArea class="flowerarea"/>
    <!-- <ButterFly class="butterfly"/> -->

  </div>
</template>

<script>

import HelloWorld from "@/components/HelloWorld.vue";
import FlowerArea from "@/components/FlowerArea.vue";
import ButterFly from "@/components/ButterFly.vue";

export default {
  name: "home",
  components: {
    HelloWorld,
    FlowerArea,
    ButterFly
  }
};
</script>
<style scoped lang="scss">
.home {
  font-family: "pink", sans-serif;
  color: #ff3cef;
  background: #33f;
}

#grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr ;
}

.helloworld {
  grid-column: 1 / 3;
  grid-row: 1 / 3;
  justify-self: center;
}

.flowerarea {
  grid-column: 1 / 3;
  grid-row: 1; 
  // background: rgb(166, 125, 156);
  // padding: 10% 2% 0.5% 2%;  
}

.butterfly{
  grid-column: 1 / 3;
  grid-row: 1 / 3; 
 }
</style>