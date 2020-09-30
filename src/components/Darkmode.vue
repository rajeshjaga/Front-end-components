<template>
  <div class="Darkmode">
    <input type="checkbox" name="checkbox" id="checkbox" />
    <div class="color">
      <label for="checkbox">
        <i class="far fa-sun"></i>
        <i class="far fa-moon"></i>
        <div class="pointer"></div>
      </label>
    </div>
  </div>
</template>

<script>
export default {
  name: "Darkmode",
};
</script>

<style scoped >
@import "../stylesheets/darkmode.scss";
</style>
