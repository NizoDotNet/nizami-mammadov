<script setup lang="ts">
defineProps<{
  link: string;
  icon: string;
}>();
</script>
<template>
  <a
    :href="link"
    target="_blank"
    class="transition-transform duration-200 hover:scale-110 hover:drop-shadow-[0_0_12px_rgba(249,115,22,0.4)]"
  >
    <UIcon :name="icon" class="text-orange-500 w-9 h-9"></UIcon>
  </a>
</template>
