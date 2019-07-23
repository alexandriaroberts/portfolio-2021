<template>
  <div id="app">  
    <Header/>
    <router-view />
    <!-- <Icons class="icon"/> -->
    <Footer class="footer"/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
// import Icons from "./components/animatedicons/Icons";
import main from "./assets/css/main.scss";

export default {
  name: "home",
  components: {
  //  Icons,
   Header,
   Footer   
  }
}
</script>

