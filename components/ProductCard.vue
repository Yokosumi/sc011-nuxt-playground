<script setup lang="ts">
import type { Product } from '../types';

type props = {
  product: Product;
};

const { product } = defineProps<props>();
</script>

<template>
  <section
    :v-for="product"
    class="flex flex-col shadow-md bg-white p-6 rounded-md"
  >
    <img class="w-[75px] h-auto self-center" :src="product.image" alt="" />
    <h2 class="text-black mt-auto text-sm">
      {{ product.title }}
    </h2>
  </section>
</template>
