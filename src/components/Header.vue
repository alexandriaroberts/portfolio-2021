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
import main from '../assets/css/main.scss'

export default {
  name: 'home',
  components: {}
}
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

header {
  grid-row: 1;
  grid-column: 5 / 9;
  justify-self: center;
  @include respond(phone) {
    grid-column: 1 / -1;
  }
}
</style>
