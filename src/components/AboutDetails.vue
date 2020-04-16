<template>
  <section class="about">
    <h2 class="heading-primary">
      ABOUT<br /><span class="underline">me</span>
    </h2>
    <div class="side__line">
      <svg
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
      </svg>
    </div>

    <div class="about-text">
      <p class="paragraph">
        Hello, I am Lexie, a Front-End Developer. I love working with CSS,
        JavaScrit and VueJs. I have worked on variety oof projects for work and
        personal projects, where I could quickly pick up new frameworks and
        languages. Please look at my projects section.
      </p>
      <p class="paragraph">
        In my spare time, I love visiting nature, going for long swims, and
        cooking.
      </p>
      <p class="paragraph">
        If you would like to find out more about me, my skills and how I can fit
        into your team please feel free to message me. I love talking about
        code, so even if you aren’t looking for a new team member right now, I
        would love to connect with you so I can share my interests and passions
        with other like minded people.
      </p>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

.about {
  grid-row: 2;
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
    margin-bottom: -6.5rem;

    @include respond(phone) {
    margin-bottom: -1.5rem;

    }
    svg {
      top: 4%;
    }
  }

  &-text {
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
