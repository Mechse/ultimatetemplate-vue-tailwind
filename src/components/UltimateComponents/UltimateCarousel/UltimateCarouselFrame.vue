<template>
  <div class="h-72 flex items-center p-4 md:px-16">
    <div class="glide flex justify-center items-center h-full">
      <div class="glide__track h-full" data-glide-el="track">
        <ul class="glide__slides h-full">
          <UltimateCarouselComponent :show-button="true"></UltimateCarouselComponent>
          <UltimateCarouselComponent></UltimateCarouselComponent>
          <UltimateCarouselComponent></UltimateCarouselComponent>
        </ul>
      </div>
      <div class="glide__arrows" data-glide-el="controls">
        <button class="glide__arrow glide__arrow--left" data-glide-dir="<">prev</button>
        <button class="glide__arrow glide__arrow--right" data-glide-dir=">">next</button>
      </div>
    </div>
  </div>
</template>

<script>
import Glide from "@glidejs/glide";
import UltimateCarouselComponent from "./UltimateCarouselComponent";

export default {
  name: "UltimateCarousel",
  components: {
    UltimateCarouselComponent
  },
  mounted() {
    const config = {
      type: "carousel",
      gap: 10,
      perView: 3,
      autoplay: 0,
      hoverpause: true,
      peek: {
        before: 100,
        after: 50
      },
      breakpoints: {
        720: {
          perView: 2
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

<style scoped>
.glide__arrow.glide__arrow--left,
.glide__arrow.glide__arrow--right {
}
.glide__arrow.glide__arrow--left:hover,
.glide__arrow.glide__arrow--right:hover {
  border-color: red;
  color: red;
}
</style>