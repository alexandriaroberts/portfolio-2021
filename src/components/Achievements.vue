<template>
  <section class="achievements">
    <h2 class="heading-primary">ACHIEVEMENTS<br />&</br><span class="underline">awards</span></h2>
    <div class="side__line">  <svg
            width="15"
            height="15"
            viewBox="0 0 15 15"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M15 7.5C15 11.6421 11.6421 15 7.5 15C3.35786 15 0 11.6421 0 7.5C0 3.35786 3.35786 0 7.5 0C11.6421 0 15 3.35786 15 7.5Z"
              fill="rgb(196, 23, 23)"
            />
          </svg></div>
      <div class="achievement-text">
      <p class="paragraph">
        <!-- <img src="../assets/images/wave.svg"> -->
       Won a T-shirt for contributing to open source issue of &rarr; <a href="https://www.vuevixens.org/" class="link" target="_blank">Vue Vixen</a>.
      </p>
      <p class="paragraph">
        Proudest moment for me, when my pen, which is done using Nasa API and Vue.JS got featured on codepen, you can check out &rarr;

        <a href="https://codepen.io/iamlexieonearth/full/vwPRPY" target="_blank" class="link">the project</a> here.
      </p>
    </div>

  </section>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

.achievements {
  grid-row: 4;
  grid-column: 2 / 12;

  @include respond(tab-port){
    grid-column: 1 / -1;
  }

  display: grid;
  grid-template-columns: 20rem 1fr;
  grid-template-rows: min-content 1fr;

  .heading-primary {
    @include mainHeading;
  }

  .side__line {
    @include line;
    margin: -6.5rem 0;

    @include respond(phone) {
       margin-bottom: -1.5rem;
    }
      svg {
        top: 25%;
    }
  }
  .achievement-text {
    grid-row: 2;
    grid-column: 2;
    align-self: center;

     @include respond(phone) {
     grid-column: 1 / -1;
     margin-top: 3rem;
      }
  }
}
</style>
