<template>
  <!-- Project details -->

  <div class="project__grid">
    <div
      v-for="(project, index) in projects"
      :key="index"
      ref="projectImage"
      role="projectItem"
      class="projectImage"
    >
      <a :href="project.url" target="_blank" rel="noopener">
        <img
          :src="project.image.imageURL"
          :alt="project.image.alt"
          :title="project.name"
          class="projectImage"
        />
      </a>
      <p class="project-title">{{ project.name }}</p>
    </div>
  </div>
</template>

<script>
import main from "../assets/css/main.scss";
import { TweenMax, Power2, TimelineMax } from "gsap/TweenMax";

export default {
  data() {
    return {
      projects: [
        {
          name: "The Big Spoon",
          url: "https://thebigspoon.ca",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/c_limit,h_100,w_150/v1616050868/2E1F2560-9DBC-4F1C-99D7-D264D0ADC4C7_1_201_a.jpg",
            alt:
              "The Big Spoon, is a homemade soup pick up service"
          }
        },
          {
          name: "Rooots",
          url: "https://www.rooots.io/",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1611069221/rooots1.png",
            alt:
              "Rooots, platform for mentoring women in tech"
          }
        },
          {
          name: "Align Somatics Movement",
          url: "https://www.alignsomatics.com/",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1611068604/as.png",
            alt:
              "Align Somatics, help people to manage their stress levels with somatic movement"
          }
        },
        {
          name: "Flower VueJs Game",
          url: "https://codepen.io/iamlexieonearth/full/QYNmEa",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170890/Flower_Game_in_VueJS.png",
            alt:
              "Flower VueJs Game, player clicks on the flower and get points for clickig on them"
          }
        },
        {
          name: "Space Game with Canvas",
          url: "https://codepen.io/iamlexieonearth/full/KEoMye",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170891/Space_Game_with_Canvas.png",
            alt:
              "Space Game with Canvas, player plays with key board and catches an alien"
          }
        },
        {
          name: "Nasa API VueJS",
          url: "https://codepen.io/iamlexieonearth/full/vwPRPY",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563856744/Nasa-API.png",
            alt: "Nasa API VueJS Project to render images from NaSa"
          }
        },
        {
          name: "CSS Grid Poster",
          url: "https://codepen.io/iamlexieonearth/full/aKOzyL",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562737397/poster.png",
            alt: "CSS Grid Poster"
          }
        },
        {
          name: "Product Landing Page",
          url: "https://codepen.io/iamlexieonearth/full/zLzdLJ",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562737777/product-landing-page.png",
            alt: "Product Landing Page of Dog Shoes"
          }
        },
        {
          name: "Survey Form",
          url: "https://codepen.io/iamlexieonearth/full/OEqZWJ",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170893/survey_form.png",
            alt: "Survey Form for Pizza delivery"
          }
        },
        {
          name: "Coffee Shop Page Layout",
          url: "https://codepen.io/iamlexieonearth/full/QxQbXX",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563171098/coffee-shop.png",
            alt: "Coffee Shop Page Layout with cosy vibe"
          }
        },
        {
          name: "Tribute Page",
          url: "https://codepen.io/iamlexieonearth/full/jGBRRE",
          image: {
            imageURL:
              "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563171331/Tribute_Page_for_Free_Code_Camp_CSS_Grid_Layout.png",
            alt: "Tribute Page of Dr. B R  Ambedkar"
          }
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

.project__grid {
  position: relative;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-auto-rows: 40rem;
  grid-auto-flow: dense;
  grid-row-gap: 7em;
  grid-column-gap: 5em;
  justify-self: center;
  align-self: center;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  position: relative;
  padding: 1em 0 1em 0;
}

.projectImage {
  cursor: pointer;
  display: block;
  grid-auto-flow: column;
  top: 0;
  background-size: cover;
  background-position: 50% 50%;
  transition: all 0.2s;
}

.projectImage:hover {
  transform: translateY(-3px);
}

.project-title {
  text-align: center;
  color: rgb(196, 23, 23);
  width: 100%;
  height: 12%;
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
