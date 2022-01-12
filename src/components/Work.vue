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
    <div class="work__text-apy">
      <h3 class="heading-secondary">
        APY Vision
        <span class="work-timeline">
          (Front-End Developer Intern, April 2021 - December 2021 )</span
        >
      </h3>
      <p class="paragraph">
        Working as an intern in my first crypto job, I learned a lot from the
        seniors and the team, it was a great experience!😊
      </p>
      <p class="paragraph">
        - Worked on creating a marketing site, one page apps for trends etc in
        React, Sass for the company. See marketing site here:
        <a
          href="https://apy.vision/"
          class="link"
          target="_blank"
          rel="noopener"
        >
          APY Vision</a
        >
      </p>
      <p class="paragraph">
        - Building web interfaces, features using API's, bug fixes and updating
        front-end design while moving from V1 to V2.
      </p>
      <p class="paragraph">
        - Working with storybook, creating web pages to show different types of
        protocols data and tracking.
      </p>
      <p class="paragraph">
        - Participated in daily team meetings remotely, sharing the things we
        achieved on the day before and our to do lists for the day while
        collaborating with other team members remotely.
      </p>
    </div>
    <div class="work__text-rooots">
      <h3 class="heading-secondary">
        Rooots<span class="work-timeline">
          (Front-End Developer, April 2020 )</span
        >
      </h3>
      <p class="paragraph">
        This is a project I started while working doing Mozilla's incubator
        program as a founder and team leader, with managing a team of 5, as well
        as conducting user interviews for research project to we developed on
        working a MVP using VueJS. This is an ongoing passion side project of
        mine!😊 You can check here:
        <a href="https://rooots.io/" class="link" target="_blank" rel="noopener"
          >Rooots</a
        >.
      </p>
    </div>
    <div class="work__text-1">
      <h3 class="heading-secondary">
        Joyjet Digital Space Agency<span class="work-timeline">
          (Front-End Developer, Sept 2019 - Feb 2020 )</span
        >
      </h3>
      <p class="paragraph">
        - Developed new user-facing features in languages such as HTML5, CSS and
        JavaScript.
      </p>
      <p class="paragraph">
        - Learned and worked on creating email designs using Foundation Zurb for
        clients.
      </p>
      <p class="paragraph">
        - Built reusable code in React for future use while ensuring the
        technical feasibility of UI/UX designs.
      </p>
      <p class="paragraph">
        - Created landing pages using Bootstrap and some Jquery on old projects.
        As well developed sites using Divi in Wordpress.
      </p>
      <p class="paragraph">
        - Optimizing applications for maximum speed and scalability using Google
        Developer Tools and Lighthouse.
      </p>
      <p class="paragraph">
        - Used Git extensively on all the projects, also used Bitbucket as part
        of the companies version control tool.
      </p>
      <p class="paragraph">
        - Participated in daily team meetings, sharing the things we achieved on
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
        - Writing code in one or more programming or scripting languages, such
        as HTML5, CSS or JavaScript in Word Press.
      </p>
      <p class="paragraph">
        - Deciding on the best technologies/plugins and languages for the
        project, testing sites and applications in different browsers and
        environments.
      </p>
      <p class="paragraph">
        - Problem solving, fixing bugs in existing projects.
      </p>
      <p class="paragraph">
        - Testing new features thoroughly to ensure they perform the correct
        task in all cases.
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
  grid-row: 6;
  grid-column: 2 / 12;
  .link {
    @include link;
  }

  @include respond(tab-port) {
    grid-column: 1 / -1;
  }

  display: grid;
  grid-template-columns: 20rem 1fr;
  grid-template-rows: min-content 1fr min-content min-content;

  .heading-primary {
    @include mainHeading;
  }

  .side__line {
    @include line;
    grid-row: 1 / 7;
    margin-top: -6.5rem;

    @include respond(phone) {
      margin-bottom: -1.5rem;
    }

    svg {
      top: 4%;
    }
  }

  &__text-apy {
    grid-row: 2;
    grid-column: 2;
    align-self: center;
    @include respond(phone) {
      grid-column: 1 / -1;
      margin-top: 3rem;
    }
  }

  &__text-rooots {
    grid-row: 3;
    grid-column: 2;
    align-self: center;
    margin-top: 6.5rem;
    @include respond(phone) {
      grid-column: 1 / -1;
      margin-top: 3rem;
    }
  }

  &__text-1 {
    grid-row: 4;
    grid-column: 2;
    align-self: center;
    margin-top: 6.5rem;

    @include respond(phone) {
      grid-column: 1 / -1;
      margin-top: 3rem;
    }
  }

  &__text-2 {
    grid-row: 5;
    grid-column: 2;
    align-self: center;
    margin-top: 6.5rem;

    @include respond(phone) {
      grid-column: 1 / -1;
    }
  }
}
</style>
