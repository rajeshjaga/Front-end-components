<template>
  <div id="app">
    <h3 class="app-title">
      Made By
      <a href="http://www.github.com/rajeshjaga" class="github" _target="blank"
        >Lucifer__13</a
      >
    </h3>
    <Darkmode />
  </div>
</template>

<script>
import Darkmode from "./components/Darkmode.vue";
export default {
  name: "App",
  components: {
    Darkmode,
  },
};
</script>

<style>
@import "./stylesheets/globals.scss";
</style>
