<template>
  <footer>
    <!-- Links to the Github, Codepen -->
    <ul class="link-list">
      <li class="link-list__item">
        <a
          href="https://codepen.io/iamlexieonearth/"
          class="link-list__link"
          aria-label="CodePen"
          aria-describedby="external"
        >
          <svg
            class="link-list__icon link-list__icon--codepen"
            viewBox="0 0 48 48"
            aria-hidden="true"
            focusable="false"
          >
            <use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#codepen" />
          </svg>
        </a>
      </li>
      <li class="link-list__item">
        <a
          href="https://github.com/alexandriaroberts"
          class="link-list__link"
          aria-label="GitHub"
          aria-describedby="external"
        >
          <svg
            class="link-list__icon link-list__icon--github"
            viewBox="0 0 48 48"
            aria-hidden="true"
            focusable="false"
          >
            <use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#github" />
          </svg>
        </a>
      </li>

      <li class="link-list__item">
        <a
          href="https://twitter.com/iamlexieonearth"
          class="link-list__link"
          aria-label="Twitter"
          aria-describedby="external"
        >
          <svg
            class="link-list__icon link-list__icon--twitter"
            viewBox="0 0 48 48"
            aria-hidden="true"
            focusable="false"
          >
            <use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#twitter" />
          </svg>
        </a>
      </li>
      <li class="link-list__item">
        <a
          href="https://www.linkedin.com/in/alexandria-roberts-001/"
          class="link-list__link"
          aria-label="YouTube"
          aria-describedby="external"
        >
          <svg
            class="link-list__icon link-list__icon--linkedin"
            viewBox="0 0 48 48"
            aria-hidden="true"
            focusable="false"
          >
            <use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#linkedin" />
          </svg>
        </a>
      </li>
    </ul>

    <svg
      version="1.1"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink"
      hidden
    >
      <symbol id="codepen" viewBox="0 0 48 48">
        <g transform="scale(0.046875 0.046875)">
          <path
            d="M123.429 668l344.571 229.714v-205.143l-190.857-127.429zM88 585.714l110.286-73.714-110.286-73.714v147.429zM556 897.714l344.571-229.714-153.714-102.857-190.857 127.429v205.143zM512 616l155.429-104-155.429-104-155.429 104zM277.143 458.857l190.857-127.429v-205.143l-344.571 229.714zM825.714 512l110.286 73.714v-147.429zM746.857 458.857l153.714-102.857-344.571-229.714v205.143zM1024 356v312c0 14.286-7.429 28.571-19.429 36.571l-468 312c-7.429 4.571-16 7.429-24.571 7.429s-17.143-2.857-24.571-7.429l-468-312c-12-8-19.429-22.286-19.429-36.571v-312c0-14.286 7.429-28.571 19.429-36.571l468-312c7.429-4.571 16-7.429 24.571-7.429s17.143 2.857 24.571 7.429l468 312c12 8 19.429 22.286 19.429 36.571z"
          />
        </g>
      </symbol>
      <symbol class="github" id="github" viewBox="0 0 48 48">
        <g transform="scale(0.046875 0.046875)">
          <path
            @mouseover="mouseover"
            ref="github"
            d="M512.008 12.642c-282.738 0-512.008 229.218-512.008 511.998 0 226.214 146.704 418.132 350.136 485.836 25.586 4.738 34.992-11.11 34.992-24.632 0-12.204-0.48-52.542-0.696-95.324-142.448 30.976-172.504-60.41-172.504-60.41-23.282-59.176-56.848-74.916-56.848-74.916-46.452-31.778 3.51-31.124 3.51-31.124 51.4 3.61 78.476 52.766 78.476 52.766 45.672 78.27 119.776 55.64 149.004 42.558 4.588-33.086 17.852-55.68 32.506-68.464-113.73-12.942-233.276-56.85-233.276-253.032 0-55.898 20.004-101.574 52.76-137.428-5.316-12.9-22.854-64.972 4.952-135.5 0 0 43.006-13.752 140.84 52.49 40.836-11.348 84.636-17.036 128.154-17.234 43.502 0.198 87.336 5.886 128.256 17.234 97.734-66.244 140.656-52.49 140.656-52.49 27.872 70.528 10.35 122.6 5.036 135.5 32.82 35.856 52.694 81.532 52.694 137.428 0 196.654-119.778 239.95-233.79 252.624 18.364 15.89 34.724 47.046 34.724 94.812 0 68.508-0.596 123.644-0.596 140.508 0 13.628 9.222 29.594 35.172 24.566 203.322-67.776 349.842-259.626 349.842-485.768 0-282.78-229.234-511.998-511.992-511.998z"
          />
        </g>
      </symbol>
      <symbol id="twitter" viewBox="0 0 48 48">
        <g transform="scale(0.046875 0.046875)">
          <path
            d="M1024 226.4c-37.6 16.8-78.2 28-120.6 33 43.4-26 76.6-67.2 92.4-116.2-40.6 24-85.6 41.6-133.4 51-38.4-40.8-93-66.2-153.4-66.2-116 0-210 94-210 210 0 16.4 1.8 32.4 5.4 47.8-174.6-8.8-329.4-92.4-433-219.6-18 31-28.4 67.2-28.4 105.6 0 72.8 37 137.2 93.4 174.8-34.4-1-66.8-10.6-95.2-26.2 0 0.8 0 1.8 0 2.6 0 101.8 72.4 186.8 168.6 206-17.6 4.8-36.2 7.4-55.4 7.4-13.6 0-26.6-1.4-39.6-3.8 26.8 83.4 104.4 144.2 196.2 146-72 56.4-162.4 90-261 90-17 0-33.6-1-50.2-3 93.2 59.8 203.6 94.4 322.2 94.4 386.4 0 597.8-320.2 597.8-597.8 0-9.2-0.2-18.2-0.6-27.2 41-29.4 76.6-66.4 104.8-108.6z"
          />
        </g>
      </symbol>
      <symbol id="linkedin" viewBox="0 0 430.117 430.118">
        <g>
          <path
            d="M398.355,0H31.782C14.229,0,0.002,13.793,0.002,30.817v368.471
		c0,17.025,14.232,30.83,31.78,30.83h366.573c17.549,0,31.76-13.814,31.76-30.83V30.817C430.115,13.798,415.904,0,398.355,0z
		 M130.4,360.038H65.413V165.845H130.4V360.038z M97.913,139.315h-0.437c-21.793,0-35.92-14.904-35.92-33.563
		c0-19.035,14.542-33.535,36.767-33.535c22.227,0,35.899,14.496,36.331,33.535C134.654,124.415,120.555,139.315,97.913,139.315z
		 M364.659,360.038h-64.966V256.138c0-26.107-9.413-43.921-32.907-43.921c-17.973,0-28.642,12.018-33.327,23.621
		c-1.736,4.144-2.166,9.94-2.166,15.728v108.468h-64.954c0,0,0.85-175.979,0-194.192h64.964v27.531
		c8.624-13.229,24.035-32.1,58.534-32.1c42.76,0,74.822,27.739,74.822,87.414V360.038z M230.883,193.99
		c0.111-0.182,0.266-0.401,0.42-0.614v0.614H230.883z"
          />
        </g>
      </symbol>
    </svg>
  </footer>
</template>

<script>
import { TweenMax, TimelineMax, Sine, Power1 } from "gsap";

export default {
  methods: {
    mouseover: function() {
      console.log("click fired");
      TweenMax.set(this.$refs.github, {
        visibility: "visible"
      });
      console.log("hey");
      const tl = new TimelineMax();

      tl.fromTo(
        this.$refs.github,
        0.2,
        { rotation: 45, transformOrigin: "50% 50%" },
        {
          rotation: -45,
          spin: 180,
          ease: Power1.easeInOut,
          repeat: 3,
          yoyo: true
        }
      );
    }
  }
};
</script>

<style scoped>
.link-list {
  list-style-type: none;
  margin: 0;
  padding: 0 2% 0.5% 2%;
}

.link-list__item {
  display: inline-block;
  margin: 0;
}

.link-list__link {
  align-items: center;
  display: flex;
  flex-direction: column;
  padding: 10px;
  position: relative;
  text-decoration: none;
}

.link-list__icon {
  height: 10vh;
  width: 10vw;
}

.link-list__icon--codepen {
  fill: #000;
}

.link-list__icon--github {
  fill: #24292e;
}

.link-list__icon--twitter {
  fill: #1da1f2;
}

.link-list__icon--linkedin {
  fill: rgb(199, 227, 241);
}
</style>
