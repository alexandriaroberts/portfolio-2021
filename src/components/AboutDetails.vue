<template>
  <div class="about">
    <!-- HTML for About Page, child component-->
    <img class="profile-picture" src="../assets/images/profile-picture.jpeg" />
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
      <span
        class="about__text-decoration"
      >love</span> coding, working on a problem and finding solutions to it. Since then I started learning to code while doing part-time jobs.
      I also started to work as a
      <span
        class="about__text-decoration"
      >volunteer developer</span> at
      <a href="shelovesdata.com" class="link-job">she loves data</a> to gain experinece & help with their website.<br><br>
      So far I have done few projects including this portfolio, a game in
      <span
        class="about__text-decoration"
      >VueJS</span> &
      few projects on CSS Grid. I also have found myself loving
      <span
        class="about__text-decoration"
      >JavaScript</span> despite finding it challenging at times. You can see all my code on  <span
        class="about__text-decoration"> Github </span> or <span class="about__text-decoration"> Codepen</span>. <br><br>
      Currently, I am living in Bali and looking for a junior position with a supportive team where I can expand my skills and grow as
      a developer, my interest lies in<span class="about__text-decoration"> JavaScript</span>, <span class="about__text-decoration"> SVG</span> and
      <span class="about__text-decoration">VueJS</span>. I also love working with <span class="about__text-decoration">CSS Grid</span>.
    </p>
    <p class="content paragraph__3">If you are intrested in working with me, please feel free to message me. I would love to hear from you, I need a job!😃 I love talking about code or if you need some encouragement in your coding journey, would love to talk about it or help you in your journey to be a developer too.😊</p>
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
  align-self: center;  
  justify-self: center;  
 }

.title {
  align-self: start;
  grid-column: 1;
  grid-row: 1;
}

.paragraph__1 {
  grid-column: 1;
  grid-row: 1;
  align-self: center;
 }

.paragraph__2 {
  grid-column: 1 / 3;
  grid-row: 2 / 3;
}

.paragraph__3 {
  grid-column: 1 / 3;
  grid-row: 3;
  align-self: end;
}


.content {
  max-width: 35em;
  color: var(--text-color-decoration);
}

.about__text-decoration {
  color: var(--text-color);
  text-transform: uppercase;
  font-size: 1.3rem;
}

.link-job {
  color: var(--text-color-secondary);
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
  border-radius: 5%;
}


@media (max-width: 760px) {
  .profile-picture {
    grid-column: 1 / 2;
    grid-row: 1;
    align-self: center;
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
    padding-top: 3em;
  }
}

@media (max-width: 460px) {
  .profile-picture {
    align-self: start;
    padding-top: 6em;
  }
}
</style>