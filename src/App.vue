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
      <router-link class="nav__list" to="/contact">
        <svg
          class="heading-top-decoration nav__contact"
          width="78"
          height="36"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect width="78" height="36" fill="#ACF8B8" />
        </svg>Contact
      </router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
:root {
  --main-bg-color: #b7278e;
  --spacing: 2rem;
  --text-color-decoration: #2f1773;
  --text-nav-decoration: #000;
}

html {
  background-color: var(--main-bg-color);
  overflow: hidden;
}

#app {
  display: grid;
  grid-template-columns: 0.5fr 1fr 1fr 0.5fr;
  grid-template-rows: 0.25fr 1fr 0.5fr 0.5fr;
}

#nav {
  // grid-column: 2 / 4;
  // grid-row: 3;
  // justify-items: start;
  // z-index: 1;
  padding-bottom: 5%;
  position: fixed;
  bottom: 0;
  left: 15%;
}

.nav__list {
  font-size: 1.5rem;
  line-height: 1.5;
  font-weight: 550;
  color: var(--text-nav-decoration);
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  transform: rotate(0.12deg);
  text-decoration: none;
}

.heading-top-decoration {
  position: relative;
  z-index: -1;
  top: -14px;
  left: 35px;
}


</style>
