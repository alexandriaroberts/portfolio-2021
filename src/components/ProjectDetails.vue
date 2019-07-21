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
        <img :src="project.image" :title="project.name" v-on:click="select(project.url)" alt="project.title"/>
        <p class="project-title">{{ project.name }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import main from "../assets/css/main.scss";
export default {
  data() {
    return {
      projects: [
        {
          name: "Flower VueJs Game",
          url: "https://codepen.io/iamlexieonearth/full/QYNmEa",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170890/Flower_Game_in_VueJS.png"
        },
        {
          name: "Space Game with Canvas",
          url: "https://codepen.io/iamlexieonearth/full/KEoMye",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170891/Space_Game_with_Canvas.png"
        },
        {
          name: "Nasa API VueJS",
          url: "https://codepen.io/iamlexieonearth/full/vwPRPY",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563188270/NasaAPI.png"
        },
        {
          name: "CSS Grid Poster",
          url: "https://codepen.io/iamlexieonearth/full/aKOzyL",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562737397/poster.png"
        },
        {
          name: "Product Landing Page",
          url: "https://codepen.io/iamlexieonearth/full/zLzdLJ",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562737777/product-landing-page.png"
        },
        {
          name: "Survey Form",
          url: "https://codepen.io/iamlexieonearth/full/OEqZWJ",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563170893/survey_form.png"
        },
        {
          name: "Coffee Shop Page Layout",
          url: "https://codepen.io/iamlexieonearth/full/QxQbXX",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563171098/coffee-shop.png"
        },
        {
          name: "Tribute Page",
          url: "https://codepen.io/iamlexieonearth/full/jGBRRE",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1563171331/Tribute_Page_for_Free_Code_Camp_CSS_Grid_Layout.png"
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
.title {
  align-self: start;
  grid-column: 1;
  grid-row: 1;
}
.project__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-auto-rows: auto;
  grid-auto-flow: dense;
  grid-gap: 3em;
  justify-self: center;
}

img {
  width: 100%;
  height: 300px;
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
  transition: 0.5 linear;
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
}

@media (max-width: 490px) {
 
  .title {
    text-align: center;
  }
}
</style>