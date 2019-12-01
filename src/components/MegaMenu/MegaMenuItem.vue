<template>
  <div class="relative" @mouseover="showMenu" @mouseleave="hideMenu">
    <a href="#" class="text-copy-primary hover:text-gray-600">{{name}}</a>
    <div class="absolute w-full">&nbsp;</div>
    <transition name="mega-menu-fade">
      <div
        v-show="isVisible"
        class="mega-menu absolute w-128 mt-4 bg-white text-gray-700 normal-case font-normal shadow-md rounded-lg overflow-hidden border"
      >
        <div class="flex px-6 py-8 mx-4">
          <ul class="w-1/2 px-4">
            <li class="mb-4">
              <slot name="link1"></slot>
            </li>
            <li class="mb-4">
              <slot name="link2"></slot>
            </li>
            <li class="mb-4">
              <slot name="link3"></slot>
            </li>
          </ul>
          <div class="w-1/2 px-4">
            <ul>
              <li class="mb-4">
                <slot name="link4"></slot>
              </li>
              <li class="mb-4">
                <slot name="link5"></slot>
              </li>
              <li class="mb-4">
                <slot name="link6"></slot>
              </li>
            </ul>
          </div>
        </div>
        <div class="bg-gray-200 px-8 py-8 text-md">
          <p>{{desc}}</p>
        </div>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: "MegaMenuItem",
  data() {
    return {
      isVisible: false
    };
  },
  props: ["name", "desc"],
  methods: {
    showMenu() {
      this.isVisible = true;
    },
    hideMenu() {
      this.isVisible = false;
    }
  }
};
</script>

<style scoped>
.mega-menu {
  left: -124px;
}

.mega-menu-fade-enter-active,
.mega-menu-fade-leave-active {
  transition: all 0.1s ease-in-out;
}

.mega-menu-fade-enter,
.mega-menu-fade-leave-to {
  opacity: 0;
  transform: translateY(-12px);
}
</style>
