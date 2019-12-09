<template>
  <div id="app" class="flex h-full flex-col">
    <MegaMenu></MegaMenu>
    <UltimateHero></UltimateHero>
    <UltimateCarousel></UltimateCarousel>
    <UltimateFooter></UltimateFooter>
  </div>
</template>

<script>
import UltimateNavbar from "./components/UltimateComponents/UltimateNavbar";
import UltimateFooter from "./components/UltimateComponents/UltimateFooter";
import UltimateHero from "./components/UltimateComponents/UltimateHero";
import UltimateCarousel from "./components/UltimateComponents/UltimateCarousel";
import MegaMenu from "./components/MegaMenu/MegaMenu";
export default {
  name: "App",
  components: {
    UltimateNavbar,
    UltimateFooter,
    MegaMenu,
    UltimateHero,
    UltimateCarousel
  }
};
</script>

<style>
#app {
  background-color: #e3e3e3;
}
</style>
