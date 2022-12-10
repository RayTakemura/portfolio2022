

<template>
  <!-- items-center h-screen -->
  <div class="w-full bg-gray-900 ">
    <HomePage />
    <AboutMe />
    <ExperiencePage />
  </div>
</template>
<script>
import HomePage from "./components/HomePage.vue"
import AboutMe from "./components/AboutMe.vue"
import ExperiencePage from "./components/ExperiencePage.vue"
export default {
  components: {
    HomePage,
    AboutMe,
    ExperiencePage,
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
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>