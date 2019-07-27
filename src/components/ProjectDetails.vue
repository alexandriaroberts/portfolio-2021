<template>
  <!-- Project details -->
  <div class="projects">
    <h1 class="heading title">Projects</h1>
    <div class="project__grid">
      <div
        v-for="(project, index) in projects"
        :key="index"
        ref="projectImage"
        class="projectImage"
        role="projectItem"
      >
        <img :src="project.image.imageURL" v-on:click="select(project.url)" :alt="project.image.alt" :title="project.name" />
        <p class="project-title">{{ project.name }}</p>
      </div>
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
    // animateBox() {
    //   TweenMax.to(
    //     ".grid_item",
    //     1.5,
    //     { scale: 0.95, ease: Power2.easeOut, yoyo: true },
    //     0.1
    //   );
    // }
  }
};
</script>

<style scoped lang="scss">
.project__grid {
  position: relative;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-auto-rows: auto;
  grid-auto-flow: dense;
  grid-gap: 2em;
  justify-self: center;
  align-self: center;
  padding: 3em 3em 3em 3em;
}

img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  // border-radius: 2%;
  position: relative;
}

.projectImage {
  background: rgb(196, 23, 23);
  cursor: pointer;
  // border-radius: 2%;
  display: block;
  grid-auto-flow: column;
  top: 0;
  background-size: cover;
  background-position: 50% 50%;
}

.projectImage:hover {
  transform: scaleY(1.05);
  transition: 10 ease-out;
  box-shadow: 0 1px 2px rgb(196, 23, 23), 0 8px 0px rgb(196, 23, 23);
}

.project-title {
  text-align: center;
  // line-height: 1.5;
  font-weight: 600;
  color: var(--main-bg-color);
  text-decoration: none;
  letter-spacing: 0.1em;
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