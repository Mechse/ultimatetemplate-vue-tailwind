<template>
  <div id="app" class="flex h-full flex-col">
    <UltimateNavbar></UltimateNavbar>
    <UltimateHero></UltimateHero>
    <UltimateCarousel></UltimateCarousel>
    <UltimateFooter></UltimateFooter>
  </div>
</template>

<script>
import UltimateNavbar from "./components/UltimateComponents/UltimateNavbar";
import UltimateFooter from "./components/UltimateComponents/UltimateFooter";
import UltimateHero from "./components/UltimateComponents/UltimateHero";
import UltimateHeroCarousel from "./components/UltimateComponents/UltimateHeroCarousel";
import UltimateCarousel from "./components/UltimateComponents/UltimateCarousel/UltimateCarouselFrame";
import MegaMenu from "./components/MegaMenu/MegaMenu";
export default {
  name: "App",
  components: {
    UltimateNavbar,
    UltimateFooter,
    MegaMenu,
    UltimateHero,
    UltimateHeroCarousel,
    UltimateCarousel
  }
};
</script>

<style>
#app {
}
</style>
