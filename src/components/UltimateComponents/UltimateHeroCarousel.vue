<template>
  <div class="h-screen flex items-center">
    <div class="glide flex justify-center items-center h-full">
      <div class="glide__track w-screen h-screen" data-glide-el="track">
        <ul class="glide__slides w-full h-full">
          <li
            v-for="img in backImgs"
            :key="img"
            :style="{ 'background-image'  : `url('${img}')` }"
            class="glide__slide w-full h-full"
          ></li>
          <li class="glide__slide w-full h-full"></li>
          <li class="glide__slide w-full h-full"></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Glide from "@glidejs/glide";

export default {
  name: "UltimateHeroCarousel",
  data() {
    return {
      backImgs: [
        "~@/assets/img/1.jpg",
        "~@/assets/img/2.jpg",
        "~@/assets/img/3.jpg"
      ]
    };
  },
  mounted() {
    const config = {
      type: "carousel",
      gap: 0,
      perView: 1,
      autoplay: 2500,
      hoverpause: false,
      peek: {
        before: 0,
        after: 0
      },
      breakpoints: {
        720: {
          perView: 1
        },
        600: {
          perView: 1,
          peek: {
            before: 0,
            after: 0
          }
        }
      }
    };

    new Glide(".glide", config).mount();
  }
};
</script>

<style>
</style>