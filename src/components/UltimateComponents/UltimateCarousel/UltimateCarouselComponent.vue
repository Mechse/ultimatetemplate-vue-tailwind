<template>
  <li class="glide__slide flex justify-center">
    <div
      class="w-full h-full rounded-lg flex items-end justify-end bg-cover bg-center bg-no-repeat"
      :style="{backgroundImage:`url(${require('@/assets/img/1.jpg')})`}"
    >
      <button
        v-if="showButton"
        class="text-red-500 py-2 px-4 m-6 border border-red-500 rounded shadow-lg"
      >Click</button>
    </div>
  </li>
</template>

<script>
export default {
  name: "UltimateCarouselComponent",
  props: ["showButton"],
  methods: {
    getImg(path) {
      return require(path);
    }
  }
};
</script>

<style>
</style>