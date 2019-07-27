<template>
  <div class="home">
    <!-- HomeDetails Child Component for Home Page -->
     <p><strong>Hello</strong>, I'm</p>
    <!-- HTML for Split Texting name-->
    <div role="name">
    <h1 id="name">
      <span class="color-1">A</span>
      <span class="color-2">l</span>
      <span class="color-3">e</span>
      <span class="color-4">x</span>
      <span class="color-1">a</span>
      <span class="color-2">n</span>
      <span class="color-2">d</span>
      <span class="color-3">r</span>
      <span class="color-4">i</span>
      <span class="color-1">a</span>
      <span class="color-2">&nbsp</span>
      <span class="color-1">R</span>
      <span class="color-2">o</span>
      <span class="color-3">b</span>
      <span class="color-4">e</span>
      <span class="color-1">r</span>
      <span class="color-2">t</span>
      <span class="color-2">s</span>
    </h1>
    </div>
    <p>
      I’m looking for a full time position as a
      <span class="job_name"> junior front-end developer</span>. Based in Bali, willing to relocate or work remotely.
      <!-- <h3 class="job_name">Front-End Developer</h3> -->
    </p>
    <ul role="list">
      <div>
        <li role="listitem">
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
          VueJS
        </li>
        <li role="listitem">
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
          JavaScript
        </li>
        <li role="listitem">
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
          HTML/CSS 
        </li>
      </div>
    </ul>

    <!-- <AppAnimatedIcon /> -->
  </div>
</template>

<script>
import { TimelineLite, TweenMax, Back, Bezier } from "gsap";
import main from "../assets/css/main.scss";
export default {
  name: "HelloWorld",
  components: {
   
  },
  props: {
    msg: String
  },
  mounted() {
    // Using GSAP TweenMAx plugin letters animation
    let letters = "#name span";

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
#name span {
  font-size: 3.5vw;
  font-weight: 900;
  font-family: 'Domine', serif;
  color: var( --text-color-decoration);
  transform: rotate(0.12deg);
  word-spacing: .5em;
}

.job_name {
  color: var(--text-color-decoration);
}

li {
  text-decoration: none;
  list-style: none;
}
.heading-top-decoration-home {
  position: relative;
  top: 49px;
  left: -40px;
  z-index: -1;
}

@media (max-width: 760px) {
  #name span { 
  font-size: 20px;
  }

  h1 {
  font-size: 22px;
  }
}
</style>
