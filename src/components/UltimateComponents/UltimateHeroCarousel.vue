<template>
  <div class="h-screen flex items-center">
    <div class="glide-hero glide flex justify-center items-center h-full">
      <div class="glide__track w-screen h-screen" data-glide-el="track">
        <ul class="glide__slides w-full h-full">
          <li
            v-for="(backImg, i) in backImgs"
            :key="i"
            :style="{backgroundImage:`url(${getImg(backImg)})`}"
            class="glide__slide w-full h-full bg-center bg-no-repeat bg-cover"
          ></li>
        </ul>
      </div>
      <div class="carousel-back-pointer z-10 w-full h-full absolute l-0 t-0">
        <div class="h-full w-full p-4 md:px-16 text-white flex justify-center flex-col">
          <h1 class="text-4xl md:text-6xl font-semibold">Ultimate Template</h1>
          <span class="text-2xl sm:text-2xl md:text-4xl font-medium">This Template is amazing!</span>
        </div>
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
      backImgs: ["1.jpg", "2.jpg", "3.jpg"]
    };
  },
  methods: {
    getImg(path) {
      return require(`@/assets/img/${path}`);
    }
  },
  mounted() {
    const config = {
      type: "carousel",
      gap: 0,
      perView: 1,
      autoplay: 5000,
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

    new Glide(".glide-hero", config).mount();
  }
};
</script>

<style scoped>
.carousel-back-pointer {
  cursor: default;
}
</style>