<script setup lang="ts">
defineProps<{
  text: string;
  bottomText: string;
}>();
</script>
<template>
  <div class="flex flex-col items-center text-center uppercase font-bold transition-transform duration-300 hover:scale-105">
    <h2 class="text-white text-5xl sm:text-7xl">
      {{ text }}
    </h2>
    <span class="text-zinc-600 text-xs sm:text-sm">{{ bottomText }}</span>
  </div>
</template>
