<template>
<html>
  <head></head>
  <body>
    <h2 v-if="dog_slider == cat_slider"> You are both a dog and a cat person 🐶 🐱</h2>
    <h2 v-else-if="dog_slider > cat_slider"> You are a dog person 🐶</h2>
    <h2 v-else>You are a cat person 🐱</h2>
    <p>How much do you like dogs?</p>
    <input type="range" min="0" max="100" style="width:300px;" id="dog_slider" v-model="dog_slider">
    <br>
    <p>How much do you like cats?</p>
    <input type="range" min="0" max="100" style="width:300px;" id="cat_slider" v-model="cat_slider">
  </body>
</html>
</template>

<script>
export default {
  data() {
    let dog_slider = 50;
    let car_slider = 50;
    return {
      dog_slider: dog_slider,
      cat_slider: car_slider
    };
  }
};
</script>

<style>
</style>