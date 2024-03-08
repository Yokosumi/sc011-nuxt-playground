<script lang="ts" setup>
const props = defineProps<{
  to: string;
}>();
</script>

<template>
  <NuxtLink
    :to="to"
    active-class="text-yellow-500 border-b-2 border-black transition duration-300"
  >
    <slot />
  </NuxtLink>
</template>
