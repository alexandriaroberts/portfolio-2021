<template>
  <!-- Project details -->

  <div class="project__grid">
    <div
      v-for="(project, index) in projects"
      :key="index"
      ref="projectImage"
      role="projectItem"
      class="project-item"
    >
      <div class="project-image">
        <img
          :src="project.image.imageURL"
          :alt="project.image.alt"
          :title="project.name"
          class="projectImage"
        />
      </div>
      <div class="project-info">
        <p class="project-title heading-primary">{{ project.name }}</p>
        <p class="project-description paragraph">{{ project.description }}</p>
        <p class="project-languages">
          <span class="heading-primary">Languages:</span>
          <span class="paragraph">{{ project.languages }}</span>
        </p>
        <div class="project-buttons">
          <button class="project-buttons__code">
            <a
              :href="project.btnSourceCode"
              target="_blank"
              v-if="project.btnSourceCode"
              class="link"
              >View Code</a
            >
          </button>
          <button class="project-buttons__site">
            <a :href="project.btnSite" target="_blank" class="link"
              >View site</a
            >
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          name: "React Form With API",
          url: "https://react-form-with-api.netlify.app/",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1618209902/Screenshot_2021-04-12_at_14.44.31.png",
            alt: "React form with react-hook-form and restcountrie.eu API"
          },
          description:
            "This is an example of how to use React hook form with restcountrie.eu API and the UI is done in tailwind CSS",
          languages: "ReactJS, Netlify, Netlify hosting, Restcountries.eu API",
          btnSourceCode:
            "https://github.com/alexandriaroberts/react-form-with-api",
          btnSite: "https://react-form-with-api.netlify.app/"
        },
        {
          name: "Rooots",
          url: "https://www.rooots.io/",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1611069221/rooots1.png",
            alt: "Rooots, platform for mentoring women in tech"
          },
          description:
            "This is the side project I am working on which is in VueJS, this has been very exciting project to begin with and been pushed to learn alot as a develoepr and team leader from this",
          languages: "VueJS, SCSS/SASS, Netlify hosting, Mailchimp",
          btnSourceCode: "https://github.com/Rooots-io",
          btnSite: "https://rooots.io/"
        },
        {
          name: "Flower VueJs Game",
          url: "https://codepen.io/iamlexieonearth/full/QYNmEa",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170890/Flower_Game_in_VueJS.png",
            alt:
              "Flower VueJs Game, player clicks on the flower and get points for clickig on them"
          },
          description:
            "This is fun little VueJS game, you have to click on the flower to get the points.",
          languages: "VueJS, SCSS/SASS, Netlify",
          btnSourceCode:
            "https://github.com/alexandriaroberts/FlowerGame-VueJS",
          btnSite: "https://codepen.io/iamlexieonearth/full/QYNmEa"
        },

        {
          name: "The Big Spoon",
          url: "https://thebigspoon.ca",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1616051142/2E1F2560-9DBC-4F1C-99D7-D264D0ADC4C7_1_201_a.jpg",
            alt: "The Big Spoon, is a homemade soup pick up service"
          },
          description:
            "This is an E-commerce soup pick up website I did for a client, with complete integration of payment etc, also did the design of it and I had to look into some theme code too",
          languages: "WordPress, CMS, Php, plugins ",
          btnSourceCode: "",
          btnSite: "https://thebigspoon.ca/"
        },
        {
          name: "Align Somatics Movement",
          url: "https://www.alignsomatics.com/",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1611068604/as.png",
            alt:
              "Align Somatics, help people to manage their stress levels with somatic movement"
          },
          description:
            "The client wanted to work on teh existing site, retaining soem pages, have have redesign of the homepage, etc. Interestingly, I used alot of HTML/CSS in this with also some Kajabi's features to deliver the design",
          languages: "Kajabi CMS, HTML, CSS, plugins ",
          btnSourceCode: "",
          btnSite: "https://www.alignsomatics.com/"
        },

        {
          name: "Space Game with Canvas",
          url: "https://codepen.io/iamlexieonearth/full/KEoMye",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170891/Space_Game_with_Canvas.png",
            alt:
              "Space Game with Canvas, player plays with key board and catches an alien"
          },
          description:
            "This is a space game using JavaScript and Canvas, you have to use your arrow keys to catch an alien by moving the space man",
          languages: "JavaScript, Canvas ",
          btnSourceCode:
            "https://github.com/alexandriaroberts/Space-Game-with-Canvas",
          btnSite: "https://codepen.io/iamlexieonearth/full/KEoMye"
        },
        {
          name: "Nasa API VueJS",
          url: "https://codepen.io/iamlexieonearth/full/vwPRPY",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563856744/Nasa-API.png",
            alt: "Nasa API VueJS Project to render images from NaSa"
          },
          description:
            "This project got me my first Codepen featured, doen in VueJs with Nasa API",
          languages: "VueJS, CSS, Nasa API",
          btnSourceCode: "https://github.com/alexandriaroberts/Nasa-API",
          btnSite: "https://codepen.io/iamlexieonearth/full/vwPRPY"
        }
      ]
    };
  },
  methods: {
    select(projectUrl) {
      window.location.href = projectUrl;
      console.log(projectUrl);
    }
  }
};
</script>

<style scoped lang="scss">
@import "../../src/assets/css/main.scss";

.project-item {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-auto-rows: 50rem;
  // grid-column-gap: 3em;
  grid-auto-flow: dense;
  @include respond(tab-port) {
    grid-template-columns: 1fr;
    grid-template-rows: auto auto;
  }
}
.project-info {
  @include respond(tab-port) {
    margin-top: 5rem;
    margin-bottom: 10rem;
  }
}

img {
  width: 100%;
  object-fit: cover;
  position: relative;
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.2);
}

.project-image {
  width: 100%;
  justify-self: center;
  @include respond(tab-port) {
    width: 70%;
  }
}

.projectImage {
  display: block;
  grid-auto-flow: column;
  top: 0;
  background-size: cover;
  background-position: 50% 50%;
}

.project-title {
  text-align: left;
  margin-left: 5rem;
  color: rgb(196, 23, 23);
  width: 100%;
  height: 12%;
}

.project-languages {
  margin-top: 1rem;
  margin-left: 5rem;

  .paragraph {
    padding-left: 1rem !important;
  }
}
.link {
  @include link;
}

button {
  border: none;
  background: none;
  padding-left: 5rem;
  padding-top: 2rem;
}
@media (max-width: 760px) {
  h1 {
    font-size: 22px;
  }

  .title {
    text-align: center;
  }
}

@media (max-width: 490px) {
  .title {
    text-align: center;
    padding-top: 3em;
  }
}
</style>
