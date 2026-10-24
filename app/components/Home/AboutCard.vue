<script setup lang="ts">
defineProps<{
  text: string;
  bottomText: string;
}>();
</script>
<template>
  <div class="flex flex-col items-center w-min uppercase font-bold transition-transform duration-300 hover:scale-105">
    <h2 class="text-white text-6xl sm:text-8xl">
      {{ text }}
    </h2>
    <span class="text-zinc-600">{{ bottomText }}</span>
  </div>
</template>
