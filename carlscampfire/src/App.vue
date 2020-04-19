<template>
  <div id="app">
    <landing-page/>
    <about-page/>
    <project-page/>
    <contact-page/>
  </div>
</template>

<script>
import LandingPage from './components/LandingPage.vue'
import AboutPage from './components/AboutPage.vue'
import ProjectPage from './components/ProjectPage.vue'
import ContactPage from './components/ContactPage.vue'
export default {
  name: 'App',
  components: {
    "landing-page" : LandingPage,
    "about-page" : AboutPage,
    "project-page" : ProjectPage,
    "contact-page" : ContactPage,
  }
}
</script>

<style>
* {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;

}
</style>
