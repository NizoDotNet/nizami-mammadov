<script setup lang="ts">
import Link from "./Link.vue";

type LinkProperties = {
  path: string;
  icon: string;
};

const links: LinkProperties[] = [
  {
    path: "/",
    icon: "i-material-symbols-home-outline",
  },
  {
    path: "/projects",
    icon: "i-material-symbols-folder-outline-rounded",
  },
  {
    path: "/tools",
    icon: "i-iconoir-tools",
  },
  {
    path: "/blog",
    icon: "i-carbon-blog",
  },
];
</script>

<template>
  <div
    class="flex justify-center gap-4 items-center bg-background px-4 py-2 rounded-2xl"
  >
    <div v-for="l in links" class="flex justify-center items-center">
      <Link :path="l.path">
        <UIcon class="size-6" :name="l.icon"></UIcon>
      </Link>
    </div>
  </div>
</template>
