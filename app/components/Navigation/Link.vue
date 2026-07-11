<script setup lang="ts">
defineProps<{
  path: string;
}>();
</script>
<template>
  <div>
    <NuxtLink :to="path" class="flex justify-center items-center">
      <slot></slot>
    </NuxtLink>
  </div>
</template>
