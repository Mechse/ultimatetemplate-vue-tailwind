<template>
  <nav :class="navClass" class="w-full flex items-center text-black">
    <!-- DESKTOP --->
    <div class="hidden md:flex items-center font-display w-full">
      <img class="w-20 ml-16 my-4" src="@/assets/logo.png" alt />
      <!-- Links --->
      <div class="ml-6 hover:text-gray" v-for="(link, index) in links" :key="index">
        <a
          class="text-lg font-semibold"
          :href="link.href"
          @click.prevent="scrollTo(link.href)"
        >{{ link.display }}</a>
      </div>

      <!-- Contact Button -->
      <div
        class="ml-6 py-1 px-2 border border-black rounded-lg shadow-lg hover:shadow-blg hover:text-gray hover:border-gray"
      >
        <a
          class="text-lg font-semibold"
          href="#contact"
          @click.prevent="scrollTo('#contact')"
        >Contact</a>
      </div>
    </div>
    <!-- DESKTOP END-->
    <!-- MOBILE -->
    <div class="md:hidden flex flex-col w-full z-10">
      <div class="full-w flex flex-row justify-between bg-white">
        <img class="w-10 ml-4 my-4" src="@/assets/logo.png" alt />
        <!-- burger toogle part-->
        <div @click="navToggle" class="ml-4 flex items-center flex-shrink-0 text-white">
          <svg
            id="menu"
            class="h-8 mr-4"
            :class="menuControl === 'flex' ? 'hidden' : 'block'"
            style="fill: #000;"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
          >
            <path
              d="M64 384h384v-42.666H64V384zm0-106.666h384v-42.667H64v42.667zM64 128v42.665h384V128H64z"
            />
          </svg>

          <svg
            id="cross"
            style="transform: rotate(45deg); fill: #4F6272;"
            class="h-8 mr-4"
            :class="menuControl"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
          >
            <path
              d="M416 277.333H277.333V416h-42.666V277.333H96v-42.666h138.667V96h42.666v138.667H416v42.666z"
            />
          </svg>
        </div>
      </div>

      <!-- menu part -->
      <div
        id="menu-links"
        class="w-full bg-gray-200 flex flex-wrap text-bgray"
        :class="menuControl"
      >
        <div
          class="pl-4 py-4 w-full cursor-pointer active:bg-blue-200"
          v-for="(link, index) in links"
          :key="index"
          @click.prevent="scrollTo(link.href)"
        >
          <a class="text-lg" :href="link.href">{{ link.display }}</a>
        </div>
        <div class="pl-4 py-4 w-full cursor-pointer active:bg-blue-200">
          <a class="text-lg" href="#">Contact</a>
        </div>
      </div>
      <!-- -->
    </div>
  </nav>
</template>

<script>
export default {
  name: "UltimateNavbar",
  data() {
    return {
      navClass: {
        "bg-white": false,
        "bg-transparent": true,
        "z-0": true,
        "z-10000": false,
        "shadow-lg": false,
        fixed: false
      },
      menuControl: "hidden",
      links: [
        { href: "#hero", display: "Home" },
        { href: "#about-us h2", display: "About us" },
        { href: "#places", display: "Places" },
        { href: "#tours", display: "Tours" }
      ]
    };
  },

  methods: {
    onScroll() {
      if (window.scrollY > 50) {
        this.navClass["bg-transparent"] = false;
        this.navClass["bg-white"] = true;
        this.navClass["z-10000"] = true;
        this.navClass["z-0"] = false;
        this.navClass.fixed = true;
        this.navClass["shadow-lg"] = true;
      } else {
        this.navClass["bg-transparent"] = true;
        this.navClass["bg-white"] = false;
        this.navClass["z-10000"] = false;
        this.navClass["z-0"] = true;
        this.navClass.fixed = false;
        this.navClass["shadow-lg"] = false;
      }
    },
    navToggle() {
      this.menuControl = this.menuControl === "hidden" ? "flex" : "hidden";
    },
    scrollTo(selector) {
      /*
      if ($nuxt.$route.path === "/") {
        this.menuControl = "hidden";
        let el = document.querySelector(selector).offsetTop - 150;
        window.scroll({ top: el, behavior: "smooth" });
      } else {
        this.$router.push("/");
      }*/
    }
  },
  mounted() {},
  beforeMount() {
    window.addEventListener("scroll", this.onScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.onScroll);
  }
};
</script>

<style scoped>
.z-10000 {
  z-index: 10000 !important;
}
</style>