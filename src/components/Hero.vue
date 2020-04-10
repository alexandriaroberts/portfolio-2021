<template>
  <div class="hero">
    <!-- HTML for Split Texting name-->

    <h1 class="hero__name">
      <span class="hero__name-first">A</span>
      <span class="hero__name-first">l</span>
      <span class="hero__name-first">e</span>
      <span class="hero__name-first">x</span>
      <span class="hero__name-first">a</span>
      <span class="hero__name-first">n</span>
      <span class="hero__name-first">d</span>
      <span class="hero__name-first">r</span>
      <span class="hero__name-first">i</span>
      <span class="hero__name-first">a</span><br />
      <span class="hero__name-last">r</span>
      <span class="hero__name-last">o</span>
      <span class="hero__name-last">b</span>
      <span class="hero__name-last">e</span>
      <span class="hero__name-last">r</span>
      <span class="hero__name-last">t</span>
      <span class="hero__name-last">s</span>
    </h1>
    <div class="hero__image">
      <img
        src="../../src/assets/images/profile-picture.jpg"
        alt=""
        class="hero__image-picture"
      />
    </div>
    <div class="hero__line"></div>
    <h4 class="hero__job">
      Front-End Developer
    </h4>
  </div>
</template>

<script>
import { TimelineLite, TweenMax, Back, Bezier } from "gsap";
export default {
  name: "Hero",
  components: {},
  props: {
    msg: String
  },
  mounted() {
    // Using GSAP TweenMAx plugin letters animation
    let letters = ".hero__name span, hero__job-name p";

    TweenMax.staggerFrom(
      letters,
      0.7,
      { opacity: 0, y: 150, ease: Back.easeOut },
      0.1
    );
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

.hero {
  grid-row: 1;
  grid-column: 1 / -1;

  display: grid;
  grid-template-columns: 1fr 1fr 0.3fr min-content;
  grid-template-rows: min-content 5rem 1fr 5rem;

  &__name {
    grid-row: 1;
    grid-column: 1 / 2;

    // font-family: 'Playfair Display', serif;
    font-family: "Lora", serif;
    line-height: 6.7rem;
    font-weight: normal;
    font-size: 5.8rem;
    &-first {
      text-transform: uppercase;
      font-style: italic;
    }
    &-last {
      border-bottom: solid 1px $color-primary;
    }
  }

  &__image {
    grid-row: 3;
    grid-column: 2 / 4;
    z-index: 2;
    margin-top: -5rem;
    &-picture {
      width: 100%;
      height: 100%;
      justify-self: stretch;
      background-size: cover;
    }
  }

  &__line {
    grid-row: 2 / -1;
    grid-column: 3 / 3;
    border-left: solid 1px $color-primary;
    border-right: solid 1px $color-primary;
    z-index: 1;
    margin-top: -5rem;
  }

  &__job {
    grid-row: 2 / -1;
    grid-column: 4 / -1;
    font-size: 2.2rem;
		font-weight: normal;
    writing-mode: vertical-rl;
    text-orientation: mixed;
    justify-content: start;
}
}
</style>
