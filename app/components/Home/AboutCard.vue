<script setup lang="ts">
defineProps<{
  text: string;
  bottomText: string;
}>();
</script>
<template>
  <div class="flex flex-col items-center w-min uppercase font-medium">
    <h2 class="text-white text-2xl md:text-4xl xl:text-7xl">
      {{ text }}
    </h2>
    <span class="text-gray-200">{{ bottomText }}</span>
  </div>
</template>
