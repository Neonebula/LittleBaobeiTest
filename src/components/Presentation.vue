<template>
  <div class="presentation">
    <h1>Little Baobei</h1>
    <Carousel :autoplay="true" :perPage="1">
      <Slide>
        <img src="../assets/burger_on_table.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/chicken_burger.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/front_shop.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/front_shop_2.jpeg" />
      </Slide>
      <Slide>
        <img src="../assets/hold_burger.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/interior.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/little_baobei_logo.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/multiple_burger.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/pink_burger.jpg" />
      </Slide>
      <Slide>
        <img src="../assets/tea_matcha.jpg" />
      </Slide>
    </Carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
export default {
  name: "Presentation",
  components: {
    Carousel,
    Slide
  }
};
</script>

<style scoped>
img {
  height: 300px;
}
</style>
