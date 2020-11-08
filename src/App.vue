<template>
  <div id="app">
    <!-- <i class="fas fa-robot"></i>
    <i class="fas fa-arrow-left"></i>
    <i class="fas fa-arrow-right"></i>-->

    <!-- <font-awesome-icon :icon="['fas', 'arrow-circle-left']" />
    <font-awesome-icon :icon="['fas', 'arrow-circle-right']" /> -->
    <Slider></Slider>
  </div>
</template>

<script>
import Slider from "./components/Slider.vue";

export default {
  name: "App",
  components: {
    Slider,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
