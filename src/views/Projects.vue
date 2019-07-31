<template>
  <div class="project-details">
    <ProjectDetails class="ProjectDetails" />
  </div>
</template>

<script>
import ProjectDetails from "../components/ProjectDetails";
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
  grid-row: 2 / 5;


  }

// .MorphingArea {
//   // position: relative;
//   grid-column: 2;
//   grid-row: 1 / 4;
// }


@media (max-width: 490px) {
.project-details {   
  grid-column: 1 / 5;
  grid-row: 1 / 5;
  // padding-top: 5rem; 
 justify-self: center;
  }
}
</style>