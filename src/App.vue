<template>
  <div id="app" class="flex h-full flex-col">
    <MegaMenu></MegaMenu>
    <UltimateHero></UltimateHero>
    <UltimateFooter></UltimateFooter>
  </div>
</template>

<script>
import UltimateNavbar from "./components/UltimateComponents/UltimateNavbar";
import UltimateFooter from "./components/UltimateComponents/UltimateFooter";
import UltimateHero from "./components/UltimateComponents/UltimateHero";
import MegaMenu from "./components/MegaMenu/MegaMenu";
/*
    UltimateNavbar,
    UltimateFooter,
    MegaMenu,
    UltimateHero
*/
export default {
  name: "App",
  components: {
    UltimateNavbar,
    UltimateFooter,
    MegaMenu,
    UltimateHero
  }
};
</script>

<style>
#app {
  background-color: #e3e3e3;
}
</style>
