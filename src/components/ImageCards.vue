<script>
export default {
  data() {
    let image_counter = 0;
    return {
      img_array: [
        "https://drive.google.com/uc?export=view&id=1vP9Aaj5toBsqRtjvBujipxxX5N_5Fj4X",
        "https://drive.google.com/uc?export=view&id=1OzQgLC2CiVqw8KwZuW6Q1mRLr3suoMdl"
      ],
      image_counter: image_counter
    };
  }
};
</script>

<template>
<html>
  <head>
    <link rel="stylesheet" href="/static/bootstrap.min.css">
  </head>
  <body>
    <div class="card">
      <img :src="img_array[image_counter]" alt="Avatar" style="width:100%;">
      <div class="container">
        <h4>
          <b>Nala</b>
        </h4>
        <p>The most wonderful pet</p>
      </div>
    </div>
    <button @click="image_counter = (image_counter + 1) % img_array.length;">Change pic!</button>
  </body>
</html>
</template>

<style>
.card {
  width: 15%;
  margin: 20px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  display: inline-block;
}
</style>