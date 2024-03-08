<script lang="ts" setup></script>

<template>
  <ul
    class="flex gap-4 p-4 bg-gradient-to-r from-indigo-500 to-red-300 rounded container mx-auto mt-2 justify-center text-xl font-mono"
  >
    <li>
      <NuxtLink to="/" active-class="text-red-500">Home</NuxtLink>
    </li>
    <li>
      <NuxtLink to="/about" active-class="text-red-500">About</NuxtLink>
    </li>
  </ul>
</template>

<style scoped>
.nuxt-link-active {
  color: red;
}
</style>
