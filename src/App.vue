<template>
  <div id="app">
    <Header />
    <router-view />
    <Footer class="footer" />
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
import main from "./assets/css/main.scss";

export default {
  name: "home",
  components: {
    Header,
    Footer
  }
};
</script>
<style scoped>
/* Main app Grid*/
#app {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: 5vh 1fr 5vh;
  grid-gap: 13rem 0;
}
</style>
