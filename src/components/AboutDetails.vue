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
        My name is
        <span class="about__text-decoration">Lexie</span> and I am a
        <span class="about__text-decoration">Front-end developer</span>.
        <br />
        <br />Since completing my
        <span class="about__text-decoration">Computer Science Engg. degree</span> at Amaravati University in India.
        I have been on a bit of a journey, at the time I wasn’t really sure if Computer
        science was for me but from it I got the opportunity to study for my masters
        degree in
        <span class="about__text-decoration">International Management</span> at the
        <span class="about__text-decoration">University of Sussex</span> on a full
        <span class="about__text-decoration">scholarship</span>.
      </p>

      <p class="content paragraph__2">
        Since then I have been working in a variety of jobs from waitressing,
        to working as a personal assistant, a club promoter and an administrator
        for a financial company. In every job, I learned and grew as a person
        and professional, and I really enjoyed every one of them, but I felt there
        was something missing and in the last couple of years I have been thinking
        more and more about coding, computer science, and how I
        <span class="about__text-decoration">loved mathematics</span>
        and
        <span class="about__text-decoration">finding solutions to complex problems</span>.
        <br />
        <br />
        <br />I started teaching myself to code again while working part-time in a variety of jobs.
        In this time, I have been mainly focussing on
        <span class="about__text-decoration">Javascript</span> and
        <span class="about__text-decoration">VueJs</span> but
        I also love working with
        <span class="about__text-decoration">CSS</span> (particularly
        <span class="about__text-decoration">CSS Grid</span>). I have completed
        a number of personal projects, which you can see on my
        <span class="about__text-decoration">Github</span> and
        <span class="about__text-decoration">Codepen</span>,
        and volunteered my time and expertise at
        <a href="https://shelovesdata.com/" target="_blank" class="link-job">SHE LOVES DATA</a> to gain experience
        & help with them with their website.
        <br />
        <br />
        <br />So now I have come full circle and I am looking for a new role as a
        <span class="about__text-decoration">Frontend Developer</span>
 in a supportive team where I can utilise my skills and grow as a developer.
        <br />
        <br />
        <br />
In my spare time, I love visiting nature, going for long swims, and cooking.
        <br />
        <br />
        <br />If you would like to find out more about me, my skills and how I can fit into your team please feel free to message me. I love talking about code, so even if you aren’t looking for a new team member right now, I would love to connect with you so I can share my interests and passions with other like minded people.
      </p>
      <p class="content paragraph__3">
        <span class="about__text-decoration">P.S.</span> And if you are reading this and thinking about starting your own coding journey, please reach out. I would love to chat, offer encouragement and
        <span class="about__text-decoration">help</span> in any way I can.
      </p>
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
  padding: 0 3em;
}

.profile-picture {
  grid-column: 2;
  grid-row: 1;
  align-self: center;
  justify-self: center;
  
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
  color: var(--text-color-decoration);
}

.link-job {
  color: var(--text-color-secondary);
  /* font-style: italic; */
  font-size: 1.1rem;
  text-transform: uppercase;
}

.link-job:hover {
  text-decoration: underline;
}

@media (max-width: 960px) {

  .profile-picture {
    grid-column: 1 / 3;
    grid-row: 1;
    align-self: start;
    padding: 2em;
  }
  
  .paragraph__1 {
    grid-column: 1 / 3;
    grid-row: 1;
    align-self: end;
    justify-self: center;
    padding-top: 15em;
  }


  .paragraph__2 {
    grid-column: 1 / 3;
    grid-row: 2 / 3;
    align-self: center;
  }

  .paragraph__3 {
    grid-column: 1 / 3;
    grid-row: 3;
    align-self: end;
  }

  .title {
    justify-self: center;
  }

  h1 {
    font-size: 22px;
  }

  img {
    width: 250px;
    height: 250px;
    object-fit: cover;
  }

  

  .content {
    max-width: 25em;
    
  }
}

@media (max-width: 460px) {
  .about {
    padding: 0;
  
  }
  .profile-picture {
    align-self: start;
    padding-top: 3em;
  }

  .title {
    text-align: center;
  }

   .content {
    max-width: 15em;
    padding-top: 0em;
    justify-self: center;
  }
}
</style>