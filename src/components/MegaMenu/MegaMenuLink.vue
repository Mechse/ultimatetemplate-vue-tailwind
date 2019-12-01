<template>
  <a :href="href" class="flex items-center group mb-8">
    <slot></slot>

    <span class="ml-4">
        <span class="block font-bold text-blue-800 group-hover:text-blue-800">
             {{title}}
        </span>
        <span class="block text-sm text-gray-600 group-hover:text-blue-800">
            {{subtitle}}
        </span>
    </span>
  </a>
</template>

<script>
export default {
  name: "MegaMenuLink",
  props: ["href", "title", "subtitle"]
};
</script>

<style></style>
