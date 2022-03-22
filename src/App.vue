<template>
  <div id="app">
    <HeaderDC msg="Welcome to Your Vue.js App" />
    <Main msg="Welcome to Your Vue.js App" />
    <Footer msg="Welcome to Your Vue.js App" />



  </div>
</template>

<script>
import HeaderDC from "./components/HeaderDC.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";





export default {
  name: "App",
  components: {
    HeaderDC,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Roboto, sans-serif;
}
</style>
