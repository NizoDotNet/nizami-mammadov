<script setup lang="ts">
defineProps<{
  upperText: string;
  bottomText: string;
}>();
</script>
<template>
  <div class="flex flex-col lg:items-start items-center">
    <h1
      class="font-bold leading-[0.95] text-white text-6xl sm:text-7xl xl:text-9xl"
    >
      {{ upperText }}
      <span class="block font-bold text-zinc-700">{{ bottomText }}</span>
    </h1>
    <slot />
  </div>
</template>
