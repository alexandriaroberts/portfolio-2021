<template>
  <!-- Header navigation-->
  <header id="nav">
    <router-link class="nav__list" to="/">
      Home
    </router-link>

    <router-link class="nav__list" to="/projects">
      Projects
    </router-link>
  </header>
</template>

<script>
// import Icons from "./components/animatedicons/Icons";
import main from "../assets/css/main.scss";

export default {
  name: "home",
  components: {}
};
</script>

<style lang="scss">
header {
  grid-row: 1;
  grid-column: 5 / 9;
}
</style>
