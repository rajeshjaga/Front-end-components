<template>
  <div id="app">
    <h3 class="app-title">
      Made By
      <a href="http://www.github.com/rajeshjaga" class="github" _target="blank">Lucifer__13</a>
    </h3>
    <Temo />
  </div>
</template>

<script>
import Temo from "./components/Temo.vue";
export default {
  name: "App",
  components: {
    Temo
  }
};
</script>

<style>
*,
*:after,
*:before {
  margin: 0;
  padding: 0;
}
.app-title {
  font-family: "Playfair Display", serif;
  position: absolute;
  bottom: 2em;
  right:1em;
}
.github {
  text-decoration: none;
  color: rgb(19, 189, 189);
}
</style>
