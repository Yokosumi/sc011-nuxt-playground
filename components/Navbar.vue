<script lang="ts" setup>

</script>

<template>
  <div>
    <h1>Navbar</h1>
  </div>
</template>

<style scoped>

div {
  padding: 1.5rem;
  background-color: moccasin;
  font-size: large;
  h1 {
    color: black;
    font-weight: 600;
    font-size: 2rem;
    width: fit-content;
    border-radius: 8%;
    padding: 0.5rem;
    background-color: green;
    &:hover {
      background-color: black;
      color: green;
      transition: background-color 0.5s, color 0.5s ease-in;
    }
  }
}

</style>
