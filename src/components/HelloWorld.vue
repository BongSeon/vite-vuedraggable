<template>
  <div class="flex flex-col items-center">
    <img src="/tailwindcss.svg" class="logo" alt="Tailwind CSS logo" />
    <p class="text-3xl text-cyan-200">{{ msg }}</p>
  </div>
</template>

<script setup lang="ts">
defineProps<{ msg: string }>()
</script>

<style scoped>
.logo {
  @apply w-24;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 1em #78cbffaa);
}
</style>
