<template>
  <div class="hello"> 
    <h1>Hello, I'm</h1>
    <!-- HTML for Split Texting name-->  
    <div id="name">
      <span class="color-1">A</span>
      <span class="color-2">L</span>
      <span class="color-3">E</span>
      <span class="color-4">X</span>
      <span class="color-1">A</span>
      <span class="color-2">N</span>
      <span class="color-2">D</span>
      <span class="color-3">R</span>
      <span class="color-4">I</span>
      <span class="color-1">A</span>
      <span class="color-2">&nbsp</span>
      <span class="color-1">R</span>
      <span class="color-2">O</span>
      <span class="color-3">B</span>
      <span class="color-4">E</span>
      <span class="color-1">R</span>
      <span class="color-2">T</span>
      <span class="color-2">S</span>
      
    </div>
    <h1> & I'm Looking For a Front-End Developer Job</h1>
     <AppAnimatedIcon/>
    </div>
</template>

<script>
import { TimelineLite, TweenMax, Back, Bezier } from "gsap";
import AppAnimatedIcon from './icons/AppAnimatedIcon.vue'
export default {
  name: "HelloWorld",
  components: {
      AppAnimatedIcon
  },
  props: {
    msg: String
  },
  mounted() {
    // Using GSAP TweenMAx plugin letters animation
   let letters = "#name span";

    TweenMax.staggerFrom(
      letters,
      1.5,
      { opacity: 0, y: 150, ease: Back.easeOut },
      0.15
    );
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hello { 
  font-family: 'Vidaloka', serif;
  color: #fefefe;  
  text-shadow: 0.5px 0.5px rgb(20, 18, 20);
  line-height: 1;
}

#name {
   
  padding: 0.5% 2% 0.5% 2%;

}
#name span {
  font-size: 5vw;
  font-weight: 600;
  // color: #33f;
}

h1 {
 font-family: 'Vidaloka', serif;
 font-size: 6vw;
 font-weight: 600;
 padding: 0.5% 2% 0.5% 2%;
}
.color-1 {
  color: #ff3cef;
}
.color-2 {
  color: #ffde11;
}
.color-3 {
  color: #fefefe;
}
.color-4 {
  color: #ff3b11;
}

</style>
