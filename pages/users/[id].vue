<script setup>
const route = useRoute();
console.log(route.params);
</script>

<template>
  <div>
    <p>Category: # {{ $route.params.id }}</p>
  </div>
</template>
