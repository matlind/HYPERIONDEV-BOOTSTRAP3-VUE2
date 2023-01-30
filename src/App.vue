<template>
  <div id="app">
    <NavBar />
    <CardMedia />
    <CourseSummary />
    <OtherBootcamps />
    <CodingJourney />
    <GetInformation />
    <GetUpgrade />
    <OpenProfile />
  </div>
</template>

<script>
import NavBar from './components/NavBar'
import CourseSummary from './components/CourseSummary.vue';
import CardMedia from './components/CardMedia.vue';
import OtherBootcamps from './components/OtherBootcamps.vue';
import CodingJourney from './components/CodingJourney.vue';
import GetInformation from './components/GetInformation.vue';
import GetUpgrade from './components/GetUpgrade.vue'
import OpenProfile from './components/OpenProfile.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    CourseSummary,
    CardMedia,
    OtherBootcamps,
    CodingJourney,
    GetInformation,
    GetUpgrade,
    OpenProfile
}
}
</script>

<style>
@import '~bootstrap/dist/css/bootstrap.css';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
