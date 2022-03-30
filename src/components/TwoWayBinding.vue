<template>
<html>
  <head></head>
  <body>
    <div>
      <p>What is your pet's name?</p>
      <p>
        <input v-model="message" placeholder="name">
      </p>
      <p>Your pet's name is: {{ message }}</p>
    </div>
  </body>
</html>
</template>

<script>
export default {
  data() {
    return {
      message: "Nala"
    };
  }
};
</script>

<style>
</style>