<template>
  <div id="app">
    <div id="nav">
      <router-link class="nav__list" to="/">
        <svg
          class="heading-top-decoration nav__home"
          width="78"
          height="36"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect width="78" height="36" fill="#ACF8B8" />
        </svg>Home
      </router-link>
      <router-link class="nav__list" to="/about">
        <svg
          class="heading-top-decoration nav__about"
          width="78"
          height="36"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect width="88" height="36" fill="#ACF8B8" />
        </svg>About
      </router-link>
      <router-link class="nav__list" to="/projects">
        <svg
          class="heading-top-decoration nav__projects"
          width="78"
          height="36"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect width="78" height="36" fill="#ACF8B8" />
        </svg>Projects
      </router-link>
     
    </div>
    <router-view />
  </div>
</template>

<script>
import main from "./assets/css/main.scss";
export default {
  
}
</script>

<style lang="scss">

.heading-top-decoration {
  position: relative;
  z-index: -1;
  top: -14px;
  left: 35px;
}
</style>