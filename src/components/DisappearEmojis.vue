<template>
<html>
  <head></head>
  <body>
    <div>
        <h1 v-if="disappear == 0"> 🐶 🐱 🐶 🐱 🐶 🐱 🐶 🐱</h1>
    </div>
    <button @click="disappear = (disappear + 1) % 2;">Surpirse!</button>
  </body>
</html>
</template>

<script>
export default {
  data() {
      let disappear = 0;
    return {
        disappear: disappear
    };
  }
};
</script>

<style>
</style>