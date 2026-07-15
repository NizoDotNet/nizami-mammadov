<script setup lang="ts">
defineProps<{
  link: string;
  icon: string;
}>();
</script>
<template>
  <a :href="link" target="_blank">
    <UIcon :name="icon" class="text-orange-500 w-9 h-9"></UIcon>
  </a>
</template>
