<script setup lang="ts">
import Link from "./Link.vue";

type LinkProperties = {
  path: string;
  icon: string;
};

const links: LinkProperties[] = [
  {
    path: "/",
    icon: "i-lucide-home",
  },
  {
    path: "/#projects",
    icon: "i-lucide-folder-code",
  },
  {
    path: "/#tools",
    icon: "i-lucide-wrench",
  },
  // {
  //   path: "/#blog",
  //   icon: "i-lucide-file-text",
  // },
];
</script>

<template>
  <nav
    class="flex justify-center gap-1 sm:gap-2 items-center bg-background/80 backdrop-blur px-2 sm:px-3 py-1.5 rounded-full border border-white/10 shadow-lg shadow-black/30"
  >
    <div v-for="l in links" :key="l.path" class="flex justify-center items-center">
      <Link :path="l.path">
        <UIcon class="size-5 sm:size-6" :name="l.icon"></UIcon>
      </Link>
    </div>
  </nav>
</template>
