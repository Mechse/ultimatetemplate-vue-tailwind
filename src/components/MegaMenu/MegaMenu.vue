<template>
  <nav class="w-full mb-4 bg-white flex flex-row justify-between shadow-md">
    <div class="logo flex items-center p-6 pl-16">
      <img class="w-16" src="../../assets/logo.png" alt />
      <p class="logo-text text-xl font-semibold ml-2">Vue JS</p>
    </div>
    <div
      class="h-full pr-24 navigation flex flex-row justify-around items-center text-lg font-semibold text-gray-700 uppercase"
    >
      <div class="navigation-item mx-4">
        <MegaMenuItem
          desc="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Atque suscipit non incidu. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Atque suscipit non incidu."
          name="Features"
        >
          <template v-slot:link1>
            <MegaMenuLink href="#" title="HEllo" subtitle="...from the otherside">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M32 96v256h448V96H32zm160.5 224h-80.4c0-26.6-21.5-48.1-48.1-48.1V192c35.3 0 64-28.7 64-64h64.5c-19.9 23.5-32.5 57.8-32.5 96s12.6 72.5 32.5 96zM448 271.9c-26 0-48 21.5-48 48.1h-80.5c19.9-23.5 32.5-57.8 32.5-96s-12.6-72.5-32.5-96H384c0 35.3 28.7 64 64 64v79.9zM32 384h448v32H32z"
                />
              </svg>
            </MegaMenuLink>
          </template>
          <template v-slot:link2>
            <MegaMenuLink href="#" title="Analytics" subtitle="Meassure your Website.">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M379.4 178.3l-87.2 133.4C299 320 303 330.5 303 342c0 26.5-21.5 48-48 48s-48-21.5-48-48c0-3 .3-6 .8-8.9l-57.6-33.5c-8.6 8.3-20.3 13.4-33.3 13.4-8.6 0-16.6-2.3-23.6-6.2L32 364.2v57.2c0 23.5 19.2 42.7 42.7 42.7h362.7c23.5 0 42.7-19.2 42.7-42.7V208.8l-58.6-38.9c-8.1 6.3-18.3 10.1-29.4 10.1-4.4 0-8.7-.6-12.7-1.7z"
                />
                <path
                  d="M117 217c26.5 0 48 21.5 48 48 0 2.1-.2 4.2-.4 6.2l60.1 33.6c8.3-6.8 18.8-10.8 30.4-10.8 3.6 0 7.1.4 10.4 1.1l87.4-135.4c-5.6-7.8-8.9-17.4-8.9-27.8 0-26.5 21.5-48 48-48s48 21.5 48 48c0 3.9-.5 7.7-1.3 11.3l41.3 27.6V90.7c0-23.5-19.2-42.7-42.7-42.7H74.7C51.2 48 32 67.2 32 90.7V320l40-38.3c-1.9-5.2-3-10.8-3-16.7 0-26.5 21.5-48 48-48z"
                />
              </svg>
            </MegaMenuLink>
          </template>
          <template v-slot:link3>
            <MegaMenuLink href="#" title="Analytics" subtitle="Meassure your Website.">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M379.4 178.3l-87.2 133.4C299 320 303 330.5 303 342c0 26.5-21.5 48-48 48s-48-21.5-48-48c0-3 .3-6 .8-8.9l-57.6-33.5c-8.6 8.3-20.3 13.4-33.3 13.4-8.6 0-16.6-2.3-23.6-6.2L32 364.2v57.2c0 23.5 19.2 42.7 42.7 42.7h362.7c23.5 0 42.7-19.2 42.7-42.7V208.8l-58.6-38.9c-8.1 6.3-18.3 10.1-29.4 10.1-4.4 0-8.7-.6-12.7-1.7z"
                />
                <path
                  d="M117 217c26.5 0 48 21.5 48 48 0 2.1-.2 4.2-.4 6.2l60.1 33.6c8.3-6.8 18.8-10.8 30.4-10.8 3.6 0 7.1.4 10.4 1.1l87.4-135.4c-5.6-7.8-8.9-17.4-8.9-27.8 0-26.5 21.5-48 48-48s48 21.5 48 48c0 3.9-.5 7.7-1.3 11.3l41.3 27.6V90.7c0-23.5-19.2-42.7-42.7-42.7H74.7C51.2 48 32 67.2 32 90.7V320l40-38.3c-1.9-5.2-3-10.8-3-16.7 0-26.5 21.5-48 48-48z"
                />
              </svg>
            </MegaMenuLink>
          </template>
          <template v-slot:link4>
            <MegaMenuLink href="#" title="HEllo" subtitle="...from the otherside">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M32 96v256h448V96H32zm160.5 224h-80.4c0-26.6-21.5-48.1-48.1-48.1V192c35.3 0 64-28.7 64-64h64.5c-19.9 23.5-32.5 57.8-32.5 96s12.6 72.5 32.5 96zM448 271.9c-26 0-48 21.5-48 48.1h-80.5c19.9-23.5 32.5-57.8 32.5-96s-12.6-72.5-32.5-96H384c0 35.3 28.7 64 64 64v79.9zM32 384h448v32H32z"
                />
              </svg>
            </MegaMenuLink>
          </template>
        </MegaMenuItem>
      </div>
      <div class="navigation-item mx-4">
        <MegaMenuItem desc name="Products">
          <template v-slot:link1>
            <MegaMenuLink href="#" title="HEllo" subtitle="...from the otherside">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M32 96v256h448V96H32zm160.5 224h-80.4c0-26.6-21.5-48.1-48.1-48.1V192c35.3 0 64-28.7 64-64h64.5c-19.9 23.5-32.5 57.8-32.5 96s12.6 72.5 32.5 96zM448 271.9c-26 0-48 21.5-48 48.1h-80.5c19.9-23.5 32.5-57.8 32.5-96s-12.6-72.5-32.5-96H384c0 35.3 28.7 64 64 64v79.9zM32 384h448v32H32z"
                />
              </svg>
            </MegaMenuLink>
          </template>
          <template v-slot:link2>
            <MegaMenuLink href="#" title="Analytics" subtitle="Meassure your Website.">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M379.4 178.3l-87.2 133.4C299 320 303 330.5 303 342c0 26.5-21.5 48-48 48s-48-21.5-48-48c0-3 .3-6 .8-8.9l-57.6-33.5c-8.6 8.3-20.3 13.4-33.3 13.4-8.6 0-16.6-2.3-23.6-6.2L32 364.2v57.2c0 23.5 19.2 42.7 42.7 42.7h362.7c23.5 0 42.7-19.2 42.7-42.7V208.8l-58.6-38.9c-8.1 6.3-18.3 10.1-29.4 10.1-4.4 0-8.7-.6-12.7-1.7z"
                />
                <path
                  d="M117 217c26.5 0 48 21.5 48 48 0 2.1-.2 4.2-.4 6.2l60.1 33.6c8.3-6.8 18.8-10.8 30.4-10.8 3.6 0 7.1.4 10.4 1.1l87.4-135.4c-5.6-7.8-8.9-17.4-8.9-27.8 0-26.5 21.5-48 48-48s48 21.5 48 48c0 3.9-.5 7.7-1.3 11.3l41.3 27.6V90.7c0-23.5-19.2-42.7-42.7-42.7H74.7C51.2 48 32 67.2 32 90.7V320l40-38.3c-1.9-5.2-3-10.8-3-16.7 0-26.5 21.5-48 48-48z"
                />
              </svg>
            </MegaMenuLink>
          </template>
          <template v-slot:link3>
            <MegaMenuLink href="#" title="Analytics" subtitle="Meassure your Website.">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M379.4 178.3l-87.2 133.4C299 320 303 330.5 303 342c0 26.5-21.5 48-48 48s-48-21.5-48-48c0-3 .3-6 .8-8.9l-57.6-33.5c-8.6 8.3-20.3 13.4-33.3 13.4-8.6 0-16.6-2.3-23.6-6.2L32 364.2v57.2c0 23.5 19.2 42.7 42.7 42.7h362.7c23.5 0 42.7-19.2 42.7-42.7V208.8l-58.6-38.9c-8.1 6.3-18.3 10.1-29.4 10.1-4.4 0-8.7-.6-12.7-1.7z"
                />
                <path
                  d="M117 217c26.5 0 48 21.5 48 48 0 2.1-.2 4.2-.4 6.2l60.1 33.6c8.3-6.8 18.8-10.8 30.4-10.8 3.6 0 7.1.4 10.4 1.1l87.4-135.4c-5.6-7.8-8.9-17.4-8.9-27.8 0-26.5 21.5-48 48-48s48 21.5 48 48c0 3.9-.5 7.7-1.3 11.3l41.3 27.6V90.7c0-23.5-19.2-42.7-42.7-42.7H74.7C51.2 48 32 67.2 32 90.7V320l40-38.3c-1.9-5.2-3-10.8-3-16.7 0-26.5 21.5-48 48-48z"
                />
              </svg>
            </MegaMenuLink>
          </template>
          <template v-slot:link4>
            <MegaMenuLink href="#" title="HEllo" subtitle="...from the otherside">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                class="w-8 text-blue-500 group-hover:text-blue-800"
                viewBox="0 0 512 512"
              >
                <path
                  d="M32 96v256h448V96H32zm160.5 224h-80.4c0-26.6-21.5-48.1-48.1-48.1V192c35.3 0 64-28.7 64-64h64.5c-19.9 23.5-32.5 57.8-32.5 96s12.6 72.5 32.5 96zM448 271.9c-26 0-48 21.5-48 48.1h-80.5c19.9-23.5 32.5-57.8 32.5-96s-12.6-72.5-32.5-96H384c0 35.3 28.7 64 64 64v79.9zM32 384h448v32H32z"
                />
              </svg>
            </MegaMenuLink>
          </template>
        </MegaMenuItem>
      </div>
      <div class="navigation-item mx-4">Contact</div>
      <div class="navigation-item mx-4">Products</div>
    </div>
  </nav>
</template>

<script>
import MegaMenuItem from "./MegaMenuItem";
import MegaMenuLink from "./MegaMenuLink";
export default {
  name: "MegaMenu",
  components: {
    MegaMenuItem,
    MegaMenuLink
  },
  data() {
    return {};
  }
};
</script>

<style scoped>
.navigation-item {
  cursor: pointer;
}
</style>
