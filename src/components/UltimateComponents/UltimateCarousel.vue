<template>
  <div class="h-64 flex items-center py-4">
    <div class="glide flex justify-center items-center h-full">
      <div class="glide__track border border-red-600 h-full" data-glide-el="track">
        <ul class="glide__slides h-full">
          <li class="glide__slide w-1/3 flex justify-center">
            <div class="w-full h-2/3 bg-gray-500">H</div>
          </li>
          <li class="glide__slide w-1/3 flex justify-center">
            <div class="w-full h-2/3 bg-gray-500">H</div>
          </li>
          <li class="glide__slide w-1/3 flex justify-center">
            <div class="w-full h-2/3 bg-gray-500">H</div>
          </li>
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

export default {
  name: "UltimateCarousel",
  mounted() {
    const config = {
      type: "carousel",
      perView: 3,
      breakpoints: {
        600: {
          perView: 1
        }
      }
    };

    new Glide(".glide", config).mount();
  }
};
</script>

<style>
</style>