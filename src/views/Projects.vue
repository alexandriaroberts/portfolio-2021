<template>
  <div class="project-details">
    <ProjectDetails class="ProjectDetails" />
    <!-- <MorphingArea class="MorphingArea" /> -->
  </div>
</template>

<script>
import ProjectDetails from "../components/ProjectDetails";
// import MorphingArea from "@/components/MorphingArea.vue";
import main from "../assets/css/main.scss";
export default {
  name: "projects",
  components: {
    ProjectDetails
  }
};
</script>

<style scoped lang="scss">
.project-details {   
  grid-column: 2 / 4;
  grid-row: 1 / 5;
  padding-top: 5rem;

  }

// .MorphingArea {
//   // position: relative;
//   grid-column: 2;
//   grid-row: 1 / 4;
// }
</style>