<script setup lang="ts">
import Link from "./Link.vue";
</script>

<template>
  <div
    class="flex justify-center gap-4 items-center bg-gray-700 px-4 py-2 rounded-2xl"
  >
    <div class="flex justify-center items-center">
      <Link path="/">
        <UIcon name="i-material-symbols-home-outline"></UIcon>
      </Link>
    </div>
  </div>
</template>
