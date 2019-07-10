<template>
  <div class="projects">
    <svg
      class="heading__top__decoration__about"
      width="98"
      height="36"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <rect width="98" height="36" fill="#ACF8B8" />
    </svg>
    <h1 class="heading title">Projects</h1>
    <div class="project__grid">
      <div v-for="(project, index) in projects" :key="index" ref="image">
        <img :src="project.image" :title="project.name"/>
      </div>
    </div>
  </div>
</template>

<script>
import main from "../assets/css/main.scss";
export default {
  data() {
    console.log("hey");
    //console.log(this.$refs.image_0);
    // console.log(projects.image)

    return {
      projects: [
        {
          name: "Flower VueJs Game",
          url: "https://codepen.io/iamlexieonearth/full/QYNmEa",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562729593/flower-game.png"
        },
        {
          name: "Space Game with Canvas",
          url: "https://codepen.io/iamlexieonearth/full/KEoMye",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562729593/space-game.png"
        },
        {
          name: "Nasa API",
          url: "https://codepen.io/iamlexieonearth/full/vwPRPY",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1562729592/nasa.png"
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
          name: "Magazine Layout",
          url: "https://codepen.io/iamlexieonearth/full/PaqMRV",
          image:
            "https://res.cloudinary.com/dv3lue3qa/image/upload/v1558501553/magzine1.png"
        }
      ]
    };
  },
  methods: {
    onClickingProject() {
      this.$refs.image_0 = image1;
       console.log(this.$refs);
    }
  }
};
</script>

<style scoped lang="scss">
.projects {
  grid-column: 2 / 4;
  grid-row: 2 / 4;
}

.project__grid {
  position: absolute;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr auto;
  grid-gap: 2em;
}

img {
  width: 300px;
  height: 250px;
  object-fit: cover;
}
.heading__top__decoration__about {
  position: absolute;
  top: 69px;
  left: 110px;
  z-index: -1;
}
</style>