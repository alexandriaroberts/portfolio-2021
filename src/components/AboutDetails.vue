<template>
  <div class="about">
    <img class="profile-picture" src="../assets/images/profile-picture.jpeg" />
    <svg
      class="heading-top-decoration-about"
      width="98"
      height="36"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <rect width="98" height="36" fill="#ACF8B8" />
    </svg>
    <h1 class="heading title">{{ details.title }}</h1>
    <p class="content paragraph__1">
      I am a
      <span class="about__text-decoration">self-taught developer.</span>
      <br />
      <br />I also have
      <span class="about__text-decoration">Computer Science Degree</span> which I took years ago from which awarded a full scholarship from 10,000 applicants to do
      masters degree at University Of Sussex.
    </p>

    <p class="content paragraph__2">
     Fast forward few years later, found myself working on a friends wordpress site & realised how much I
      <span class="about__text-decoration">love</span> coding, working on problem. Since then I started learning to code while doing part-time jobs.
      I also started to work as a <span class="about__text-decoration"> volunteer developer </span> at <a href="shelovesdata.com" class="link-job">she loves data</a> to gain experinece & help. So far I have done few projects including this portfolio, a game in
      <span class="about__text-decoration">VueJS</span>,
      few projects on CSS Grid. I also have found myself loving
      <span class="about__text-decoration">JavaScript</span> despite finding it challenging at times. you can see it on Github or Codepen.
      Currently, I am doing my portfolio as you see, using
      <span class="about__text-decoration">SVG</span>and
      <span class="about__text-decoration">VueJS</span>to add animations
      and create an interactive portfolio, this is what I am working on.
    </p>
  </div>
</template>

<script>
import about from "../assets/translations/about";
import main from "../assets/css/main.scss";
export default {
  data() {
    return {
      details: {
        title: "About Me"
      }
    };
  },
  methods: {
    aboutMouseoverEffect() {
      color: "red";
    }
  }
};
</script>

<style scoped>
.about {
  display: grid;
  grid-template-columns: 1fr 1fr 0.5fr;
  grid-template-rows: 1fr 1fr;
 
}

.profile-picture {
  grid-column: 2;
  grid-row: 1;
  justify-self: center;
  padding: 1em;
}

.title {
  align-self: start;
  grid-column: 1;
  grid-row: 1;
 }

.paragraph__1 {
  grid-column: 1;
  grid-row: 1;
  align-self: start;
  padding-top: 5em;
}

.paragraph__2 { 
  grid-column: 1 / 3;
  grid-row: 2 / 3;
}

.content {
  max-width: 35em;
  color: var(--text-color-decoration);
  }

.about__text-decoration {
  color: var(--text-color);
  text-transform: uppercase;
  font-size: 1.3rem;
  /* text-decoration: underline; */
}

.link-job {
  color:  #f86614;
  font-style: italic;
  font-size: 1.1rem;
  text-decoration: none;
}

.link-job:hover {
  text-decoration: underline;

}

img {
  width: 250px;
  height: 250px;
  object-fit: cover;
  border-radius: 10%;
}

.heading-top-decoration-about {
  position: absolute;
  top: 120px;
  left: 200px;
  z-index: -1;
}

@media (max-width: 760px) {
 .profile-picture {
  grid-column:  1 / 2;
  grid-row: 1;
  justify-self: center;
  padding-top: 5em;
}

img {
  width: 60vw;
  height: 50vh;
  object-fit: cover;
  border-radius: 1%;
}


.paragraph__1 {
  grid-column: 1 / 3;
  grid-row: 1;
  align-self: end;
 justify-self: center;
}

.paragraph__2 { 
  grid-column: 1 / 3;
  grid-row: 2;
 justify-self: center;
}
 
 .content {
  max-width: 25em;
  /* text-align: center; */
  padding-top: 5em;
  }
 
}

</style>