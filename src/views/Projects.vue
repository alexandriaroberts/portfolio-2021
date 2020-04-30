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
  grid-column: 1 / -1;
  grid-row: 2;
}
@media (max-width: 490px) {
  .project-details {
    grid-column: 1 / -1;
    justify-self: center;
  }
}
</style>
