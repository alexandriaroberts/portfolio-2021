<template>
  <footer>
    <!-- Footer Component-->
    <div class="content__social">
      <h2 class="heading-primary social-text">Find me here</h2>
      <div class="content__networks">
        <div class="content__network">
          <a
            href="https://twitter.com/iamlexieonearth"
            target="_blank"
            rel="noopener"
            class="content__network__link"
            ><svg class="icon" viewBox="0 0 216 216">
              <use xlink:href="../assets/images/sprite.svg#twitter"></use>
            </svg>
          </a>
        </div>
        <div class="content__network">
          <a
            href="https://github.com/alexandriaroberts"
            target="_blank"
            rel="noopener"
            class="content__github__link"
            ><svg class="icon" viewBox="0 0 216 216">
              <use xlink:href="../assets/images/sprite.svg#github"></use></svg
          ></a>
        </div>
        <div class="content__network">
          <a
            href="https://codepen.io/iamlexieonearth"
            target="_blank"
            rel="noopener"
            class="content__network__link"
            ><svg class="icon" viewBox="0 0 216 216">
              <use xlink:href="../assets/images/sprite.svg#codepen"></use></svg
          ></a>
        </div>
        <div class="about-content__network">
          <a
            href="https://www.linkedin.com/in/alexandria-roberts-57a3b8182/"
            target="_blank"
            rel="noopener"
            class="content__network__link"
            ><svg class="icon" viewBox="0 0 216 216">
              <use xlink:href="../assets/images/sprite.svg#linkedin"></use></svg
          ></a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import main from "../assets/css/main.scss";

export default {};
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

footer {
  position: relative;
  grid-column: 1 / -1;
  grid-row: 3;
  z-index: 1;
  justify-content: center;
  text-align: center;
}
.content__networks {
  position: relative;
  display: grid;
  grid-auto-flow: column;
  padding-top: 1.5em;
  text-transform: uppercase;
}

a {
  color: var(--text-color-secondary);
  font-weight: bold;
  text-decoration: none;
  padding-left: 6px;
}

.icon {
  width: 6rem;
  fill: $color-secondary;
  stroke: $color-primary;
  stroke-width: 5px;
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.2);

  transition: all 0.2s ease;
  &:hover,
  &:focus {
    fill: $color-primary;
    transform: scale(1.1) translateY(-5px);
  }
}

.social-text {
  &::before {
    content: " ";
    position: absolute;
    display: inline-block;
    width: 30%;
    height: 1px;
    left: 10%;
    top: 12%;
    background: $color-primary;
  }

  &::after {
    content: " ";
    position: absolute;
    display: inline-block;
    width: 30%;
    height: 1px;
    right: 10%;
    top: 12%;
    background: $color-primary;
  }

  .heading-primary {
    padding-right: 0 !important;
  }
}
</style>
