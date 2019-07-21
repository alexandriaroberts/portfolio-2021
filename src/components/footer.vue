<template>
  <footer>
    <!-- Footer Component-->
    <div class="about-content__social">
      <div class="about-content__social-title">You can find me here:</div>
      <div class="about-content__networks">
        <div class="about-content__network">
          <a
            href="https://twitter.com/iamlexieonearth"
            target="_blank"
            class="about-content__network__link"
          >twitter</a>
        </div>
        <div class="about-content__network">
          <a
            href="https://github.com/alexandriaroberts"
            target="_blank"
            class="about-content__network__link"
          >Github</a>
        </div>
        <div class="about-content__network">
          <a
            href="https://codepen.io/iamlexieonearth"
            target="_blank"
            class="about-content__network__link"
          >Codepen</a>
        </div>
        <div class="about-content__network">
          <a
            href="https://www.linkedin.com/in/alexandria-roberts-57a3b8182/"
            target="_blank"
            class="about-content__network__link"
          >linkedin</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import main from "../assets/css/main.scss";

export default {};
</script>

<style scoped>
footer {
  position: relative;
  grid-column: 2 / 4;
  grid-row: 5;
  z-index: 1;
  /* padding-top: 1em; */
}
.about-content__networks {
  position: relative;
  display: grid;
  grid-auto-flow: column;
  padding-top: 1.5em;
  text-transform: uppercase;
}

a {
  color: var( --text-color-secondary);
  font-weight: bold;
  text-decoration: none;
  padding-left: 6px;
}

a:hover {
  color: var(--text-color);
}

@media (max-width: 960px) {
  footer {
    grid-column: 2 / 4;
  }
}

@media (max-width: 460px) {
  footer {
    grid-column: 2 / 4;
  }
  .about-content__networks {
    grid-auto-flow: row;
    justify-content: center;
  }
}
</style>