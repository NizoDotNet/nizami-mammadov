<script setup lang="ts">
defineProps<{
  path: string;
}>();
</script>
<template>
  <div>
    <NuxtLink :to="path" class="flex w-full justify-center items-center rounded-full p-2.5 transition-all duration-200 hover:bg-white/10 hover:text-white text-zinc-300 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-white/20">
      <slot></slot>
    </NuxtLink>
  </div>
</template>
