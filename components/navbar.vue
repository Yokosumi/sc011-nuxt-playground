<script lang="ts" setup>
import CustomLink from '@/components/CustomLink.vue';
</script>

<template>
  <ul
    class="flex gap-4 p-4 bg-gradient-to-r from-indigo-500 to-red-300 rounded container mx-auto mt-2 justify-center text-xl font-mono"
  >
    <li>
      <CustomLink to="/">Home</CustomLink>
    </li>
    <li>
      <CustomLink to="/about">About</CustomLink>
    </li>
    <li>
      <CustomLink to="/books">Books</CustomLink>
    </li>
    <li>
      <CustomLink to="/products">Products</CustomLink>
    </li>
  </ul>
</template>
