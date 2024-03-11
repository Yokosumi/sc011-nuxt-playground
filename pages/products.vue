<script setup lang="ts">
import type { Product } from '../types';

const url = 'https://fakestoreapi.com/products';

const { pending, data: products } = useFetch<Product[]>(url, {
  lazy: false,
});
</script>

<template>
  <section v-if="pending">
    <p>Loading...</p>
  </section>
  <section v-else class="grid grid-cols-5 gap-4">
    <ProductCard
      v-for="product in products"
      :key="product.id"
      :product="product"
      :title="product.title"
      :image="product.image"
    />
  </section>
</template>
