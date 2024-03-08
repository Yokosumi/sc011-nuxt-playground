<script setup>
const counter = useCounter();
</script>
<template>
  <div class="w-full h-[100vh]">
    <h1>Home</h1>
    <div>
      Counter: {{ counter.count }}
      <button @click="counter.increment">+</button>
      <button @click="counter.decrement">-</button>
    </div>
  </div>
</template>

<style scoped>
button {
  @apply border-2 border-black px-4 mx-2 text-lg bg-lime-300;
}
</style>
