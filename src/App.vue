<template>
<html>
  <div class="jumbotron text-center" style="background-color:#61b0b7;">
    <br>
    <h1 style="color:white; text-align:center; margin:15px;">Pets</h1>
    <p
      style="color:white; text-align:center; margin:15px;"
    >Mariana Martínez Celis González A01194953</p>
    <br>
  </div>
  <header>
    <NavBar/>
  </header>
  <body>
    <ImageCards/>
    <br>
    <TwoWayBinding/>
    <br>
    <SlidersPets/>
    <br>
    <DogBreeds/>
    <br>
    <DisappearEmojis/>
  </body>
</html>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import ImageCards from "./components/ImageCards.vue";
import TwoWayBinding from "./components/TwoWayBinding.vue";
import SlidersPets from "./components/SlidersPets.vue";
import DogBreeds from "./components/DogBreeds.vue";
import DisappearEmojis from "./components/DisappearEmojis.vue";
export default {
  name: "App",
  components: {
    NavBar,
    ImageCards,
    TwoWayBinding,
    SlidersPets,
    DogBreeds,
    DisappearEmojis
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "montserrat", sans-serif;
  text-align: center;
}

header {
  width: 100vw;
  background-color: #16558f;
  padding: 15px;
}

jumbotron .text-center {
  text-align: center;
}
</style>