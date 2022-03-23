<template>
  <div id="app">
    <HeaderDC msg="Welcome to Your Vue.js App" />
    <MainDC msg="Welcome to Your Vue.js App" />
    <FooterDC msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
/* eslint-disable */
import HeaderDC from "./components/HeaderDC.vue";
import MainDC from "./components/MainDC.vue";
import FooterDC from "./components/FooterDC.vue";

export default {
  name: "App",
  components: {
    HeaderDC,
    MainDC,
    FooterDC,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Roboto, sans-serif;
}
</style>
