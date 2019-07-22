<template>
  <div>
    <h1 class="heading title">About Me</h1>
    <div class="about">
      <!-- HTML for About Page, child component-->
      <img
        class="profile-picture"
        src="../assets/images/profile-picture.jpeg"
        alt="Profile Picture"
      />
      <p class="content paragraph__1">
        I am Lexie and I am a
        <span class="about__text-decoration">self-taught developer.</span>
        <br />
        <br />I did take a
        <span class="about__text-decoration">Computer Science Degree</span> years ago which to be honest I don't think was that useful, but the great thing is I was awarded a full scholarship 
        from 10,000 applicants to study masters degree in International Managemnet at University Of Sussex because of it.😊✨ 
      </p>

      <p class="content paragraph__2">
        For few years, I found myself doing variety of jobs from waitressing, personal assistant, club promoter to administrator for a financial company. Almost all jobs I did I feel like
         were important for me to grow as a person and I enjoyed them very well. <br /><br> <br> 
       
          But since last couple of years I found myself doing some deep thinking & realised how much I
        <span
          class="about__text-decoration"
        >loved</span> using my brain and coding while at uni, also loved mathematics in school, working on a problem and finding solutions to it. Since then I started learning to code again while doing part-time jobs.
        I also started to work as a
        <span
          class="about__text-decoration"
        >volunteer developer</span> at
        <a href="shelovesdata.com" class="link-job">she loves data</a> to gain experinece & help with their website.
        <br /><br />
        <br />So far I have done few projects including this portfolio, a game in
        <span
          class="about__text-decoration"
        >VueJS</span> &
        few projects on CSS Grid. I also have found myself loving
        <span
          class="about__text-decoration"
        >JavaScript</span> despite finding it challenging at times. You can see all my code on
        <span
          class="about__text-decoration"
        >Github</span> or
        <span class="about__text-decoration">Codepen</span>.
        <br /><br />
        <br />Currently, I am looking for a front-end position with a supportive team where I can expand my skills and grow as
        a developer, my interest lies in
        <span
          class="about__text-decoration"
        >JavaScript</span>,
        <span class="about__text-decoration">SVG</span> and
        <span class="about__text-decoration">VueJS</span>. I also love working with
        <span class="about__text-decoration">CSS Grid</span>.
        <br/>
        <br/>
        <br/>
        In my leisure time, I love visiting nature🌳, going for long swims and cooking.🤤🥣🥗
      </p>
      <p
        class="content paragraph__3"
      >If you are intrested in working with me, please feel free to message me. I would love to hear from you, I need a job!😃 I love talking about code or if you need some encouragement in your coding journey, would love to talk about it or help you in your journey to be a developer too.😊</p>
    </div>
  </div>
</template>

<script>
import about from "../assets/translations/about";
import main from "../assets/css/main.scss";
export default {};
</script>

<style scoped>
.about {
  position: relative;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 0.5fr 1fr;
  padding:0 3em;
}

.profile-picture {
  grid-column: 2;
  grid-row: 1;
  align-self: center;
  justify-self: center;
  float: left;
}

img {
  width: 300px;
  height: 350px;
  object-fit: cover;
}

.paragraph__1 {
  grid-column: 1 / 2;
  grid-row: 1;
  align-self: center;
}

.paragraph__2 {
  grid-column: 1 / 3;
  grid-row: 2 / 3;
  align-self: start;
}

.paragraph__3 {
  grid-column: 1 / 3;
  grid-row: 3;
  align-self: end;
}

.content {
  max-width: 35em;
  color: var(--text-color);
}

.about__text-decoration {
  /* color: var(--text-color); */
  color: var(--text-color-decoration);
  font-style: italic;
}

.link-job {
  color: var(--text-color-secondary);
  /* font-style: italic; */
  font-size: 1.1rem;
  text-decoration: none;
  text-transform: uppercase;
}

.link-job:hover {
  text-decoration: underline;
}

@media (max-width: 760px) {
  .profile-picture {
    grid-column: 1 / 2;
    grid-row: 1;
    align-self: center;
  }

  .title{
    justify-self: center;
  }

  img {
    width: 250px;
    height: 250px;
    object-fit: cover;
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
    padding-top: 3em;
  }

    .title {
    text-align: center;
  }
}
</style>