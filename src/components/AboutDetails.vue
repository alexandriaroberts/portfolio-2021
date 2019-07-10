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
    <p
      class="content paragraph__1"
    >I am a <span class="about__text-decoration">self-taught developer.</span><br><br> 
   I also have<span class="about__text-decoration"> Computer Science Degree </span> which I took years ago from which awarded from 10,000 applicants a full scholarship to do 
    masters degree at University Of Sussex.  </p>
    
    <p class="content paragraph__2">
    After working on a friends wordpress site, I realised how much I <span class="about__text-decoration"> love </span> coding, working on problem. Since then I started learning to code slowly.
    So far I have done few projects including this portfolio, a game in <span class="about__text-decoration"> VueJS</span>, 
    few projects on CSS Grid. I also have found myself loving <span class="about__text-decoration">JavaScript</span> despite finding it challenging at times.  you can see it on Github or Codepen. 
    Currently, I am doing my portfolio as you see, using <span class="about__text-decoration"> SVG </span>and <span class="about__text-decoration"> VueJS </span>to add animations 
    and create an interactive portfolio, this is what I am working on. </p>
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
      color: 'red'
    }
  }
};
</script>

<style scoped>
.about {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 50px 1fr 1fr;
}

.profile-picture {
  grid-column: 2;
  grid-row: 1;
  justify-self: center;
  padding: 5em 1em 1em 0;

}

.title {
  align-self: start;
  grid-column: 1;
  grid-row: 1;
}
.paragraph__1 {
  padding: 5em 1em 1em 0;
  grid-column: 1;
  grid-row: 1; 
   align-self: end;
}

.paragraph__2 {
  padding: 0 1em 1em 1em;
  grid-column: 2;
  grid-row: 2;
}

.content {
  max-width: 30em; 
  color: var(--text-color-decoration);
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  transform: rotate(0.12deg);
}

.about__text-decoration {
  color: var(--text-color);
  text-transform: uppercase;
  font-size: 1.3rem;
  /* text-decoration: underline; */
}
.about__text-decoration:hover {
 text-decoration: underline;
 color: #F86614;
}
img {
  width: 250px;
  height: 250px;
  object-fit: cover;
  border-radius: 10%;
}

.heading-top-decoration-about {
  position: relative;
  top: 0px;
  left: -890px;
  z-index: -1;
}

</style>