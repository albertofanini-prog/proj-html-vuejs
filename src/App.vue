<template>
  <div id="app">
    <TheHeader/>
    <TheJumbotron/>
    <TheRecordsSection/>
    <TheTrailerSection/>
    <TheLatestCoursesSection/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheJumbotron from './components/TheJumbotron.vue'
import TheRecordsSection from './components/TheRecordsSection.vue'
import TheTrailerSection from './components/TheTrailerSection.vue'
import TheLatestCoursesSection from './components/TheLatestCoursesSection.vue'

export default {
  name: 'App',
  components: {
    TheHeader,
    TheJumbotron,
    TheRecordsSection,
    TheTrailerSection,
    TheLatestCoursesSection
  }
}
</script>

<style lang="scss">
*{
  margin: 0 auto;
  padding: 0;
  box-sizing: border-box;
  #app {
    font-family: "Open-sans", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
}
@font-face {
  font-family: "Open-sans";
  src: local("Open-Sans"),
  url(./font/openSans/static/OpenSans/OpenSans-Regular.ttf) format("truetype");
}
</style>
