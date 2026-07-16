<script setup lang="ts">
import AboutCard from "./AboutCard.vue";
</script>

<template>
  <div
    class="flex flex-col items-center text-center lg:items-start lg:text-left"
  >
    <h1
      class="text-4xl font-bold leading-[0.95] text-white sm:text-5xl md:text-7xl xl:text-9xl"
    >
      SOFTWARE
      <span class="block font-bold text-gray-700"> ENGINEER </span>
    </h1>

    <h4 class="ms-1 mt-4 max-w-md text-gray-400">
      Passionate about creating intuitive and engaging user experiences.
      Specialize in transforming ideas into beautifully crafted products.
    </h4>
    <div class="mt-9 flex md:gap-10 gap-6 justify-center">
      <AboutCard text="+12" bottom-text="Years of experience" />
      <AboutCard text="+45" bottom-text="Projects completed" />
      <AboutCard text="+40" bottom-text="World Wide Clients" />
    </div>
  </div>
</template>
