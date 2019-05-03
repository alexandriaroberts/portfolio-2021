<template>
  <div class="home" id="grid-container">
    <HelloWorld class="helloworld"/>
    <!-- <FlowerArea/> -->
    <ArtWork class="artwork"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import FlowerArea from "@/components/FlowerArea.vue";
import ArtWork from "@/components/ArtWork.vue";

export default {
  name: "home",
  components: {
    HelloWorld,
    FlowerArea,
    ArtWork
  }
};
</script>
<style scoped lang="scss">
.home {
  font-family: "pink", sans-serif;
  color: #33f;
  background: #fce4ec;
}

#grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
}

.helloworld {
  grid-column: 1;
  grid-row: 1 / 3;
  justify-self: center;
}

.artwork {
  grid-column: 2;
  grid-row: 1 / 3; 
  background: rgb(166, 125, 156);
  padding: 10% 2% 0.5% 2%;
}
</style>