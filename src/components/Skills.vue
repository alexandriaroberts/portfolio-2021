<template>
  <section class="skills">
    <h2 class="heading-primary">SKILLS<br />&</br><span class="underline">abilities</span></h2>
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
         <ul class="skills__list paragraph">
           <li class="skills__list-type">
              HTML/CSS
           </li>
            <li class="skills__list-type">
              JavaScript
           </li>
            <li class="skills__list-type">
              Vue.JS
           </li>
            <li class="skills__list-type">
              SSS/SASS
           </li>
            <li class="skills__list-type">
              Foundation Zurb
           </li>
            <li class="skills__list-type">
              React
           </li>
           <li>Node/ Express/ MongoDB</li>
         </ul>

  </section>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

.skills {
  grid-row: 3;
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

      svg {
        top: 25%;
    }

     @include respond(phone) {
    margin-bottom: -1.5rem;

    }
  }

  &__list {
    grid-row: 2;
    grid-column: 2;
    align-self: center;
    list-style-type: none;
    padding-left: 5rem;


     @include respond(phone) {
     grid-column: 1 / -1;
     margin-top: 3rem;
      }
      
    &-type {
      &:not(:last-child) {
        margin-bottom: 1.5rem;
	}
    }
  }
}
</style>
