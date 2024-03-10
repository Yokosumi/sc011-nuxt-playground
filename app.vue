<script setup>
import navbar from './components/navbar.vue';
</script>

<template>
  <NuxtLoadingIndicator />
  <navbar />
  <div class="mx-8 my-4">
    <NuxtPage />
  </div>
</template>
