

<template>
  <!-- items-center h-screen -->
  <div class="w-full bg-gray-900 ">
    <HomePage />
    <AboutMe />
    <ExperiencePage />
    <Footer />
  </div>
</template>
<script>
import HomePage from "./components/HomePage.vue";
import AboutMe from "./components/AboutMe.vue";
import ExperiencePage from "./components/ExperiencePage.vue";
import Footer from "./components/FooterLinks.vue";
export default {
  components: {
    HomePage,
    AboutMe,
    ExperiencePage,
    Footer,
  },
  name: 'App',
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: rgb(255 255 255);
  /* margin-top: 60px; */
}
</style>