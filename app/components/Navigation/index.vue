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
    class="flex justify-evenly md:justify-center gap-1 md:gap-2 items-center bg-background/80 backdrop-blur w-[calc(100%-2rem)] max-w-sm md:w-auto px-3 md:px-4 py-2 rounded-full border border-white/10 shadow-lg shadow-black/30"
  >
    <div v-for="l in links" :key="l.path" class="flex-1 md:flex-none flex justify-center items-center">
      <Link :path="l.path">
        <UIcon class="size-6" :name="l.icon"></UIcon>
      </Link>
    </div>
  </nav>
</template>
