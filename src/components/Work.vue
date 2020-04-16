<template>
  <section class="work">
    <h2 class="heading-primary">
      WORK<br /><span class="underline">experience</span>
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

    <div class="work__text-1">
      <h3 class="heading-secondary">
        Joyjet Digital Space Agency<span class="work-timeline">
          (Front-End Developer, Sept 2019 - Feb 2020 )</span
        >
      </h3>
      <p class="paragraph">
        Developed new user-facing features in languages such as HTML5, CSS and
        JavaScript.
      </p>
      <p class="paragraph">
        Learned and worked on creating email designs using Foundation Zurb for
        clients.
      </p>
      <p class="paragraph">
        Built reusable code in React for future use while ensuring the technical
        feasibility of UI/UX designs.
      </p>
      <p class="paragraph">
        Created landing pages using Bootstrap and some Jquery on old projects.
        As well developed sites using Divi in Wordpress.
      </p>
      <p class="paragraph">
        Optimizing applications for maximum speed and scalability using Google
        Developer Tools and Lighthouse.
      </p>
      <p class="paragraph">
        Used Git extensively on all the projects, also used Bitbucket as part of
        the companies version control tool.
      </p>
      <p class="paragraph">
        Participated in daily team meetings, sharing the things we achieved on
        the day before and our to do lists for the day while collaborating with
        other team members remotely.
      </p>
    </div>

    <div class="work__text-2">
      <h3 class="heading-secondary">
        She Loves Data<span class="work-timeline">
          (Front-End Developer, Dec 2018 - Sept 2019 )</span
        >
      </h3>
      <p class="paragraph">
        Writing code in one or more programming or scripting languages, such as
        HTML5, CSS or JavaScript in Word Press.
      </p>
      <p class="paragraph">
        Deciding on the best technologies/plugins and languages for the project,
        testing sites and applications in different browsers and environments.
      </p>
      <p class="paragraph">
        Problem solving, fixing bugs in existing projects.
      </p>
      <p class="paragraph">
        Testing new features thoroughly to ensure they perform the correct task
        in all cases.
      </p>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

.work {
  grid-row: 5;
  grid-column: 2 / 12;

  @include respond(tab-port) {
    grid-column: 1 / -1;
  }

  display: grid;
  grid-template-columns: 20rem 1fr;
  grid-template-rows: min-content 1fr min-content;

  .heading-primary {
    @include mainHeading;
  }

  .side__line {
    @include line;
    margin-top: -6.5rem;

    @include respond(phone) {
      margin-bottom: -1.5rem;
    }

    svg {
      top: 4%;
    }
  }

  &__text-1 {
    grid-row: 2;
    grid-column: 2;
    align-self: center;

    @include respond(phone) {
      grid-column: 1 / -1;
      margin-top: 3rem;
    }
  }

  &__text-2 {
    grid-row: 3;
    grid-column: 2;
    align-self: center;
    margin-top: 6.5rem;

    @include respond(phone) {
      grid-column: 1 / -1;
    }
  }
}
</style>
