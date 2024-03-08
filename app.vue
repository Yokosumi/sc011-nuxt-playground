<script setup>
import navbar from './components/navbar.vue';

const route = useRoute();
</script>

<template>
  <navbar />
  <div class="mx-8 my-4">
    <NuxtPage />
  </div>
</template>
