<script setup lang="ts"></script>

<template>
  <div
    class="flex flex-col items-center text-center lg:items-start lg:text-left"
  >
    <h1
      class="font-bold leading-[0.95] text-white text-6xl sm:text-7xl xl:text-9xl"
    >
      SOFTWARE
      <span class="block font-bold text-zinc-700"> ENGINEER </span>
    </h1>

    <h4 class="ms-1 mt-4 max-w-md text-zinc-400">
      Passionate about creating intuitive and engaging user experiences.
      Specialize in transforming ideas into beautifully crafted products.
    </h4>
    <div class="mt-9 flex md:gap-10 gap-6 justify-center">
      <HomeAboutCard text="+12" bottom-text="Years of experience" />
      <HomeAboutCard text="+45" bottom-text="Projects completed" />
      <HomeAboutCard text="+40" bottom-text="World Wide Clients" />
    </div>
    <div class="mt-14 lg:mt-28 flex flex-col gap-14 lg:gap-28">
      <HomeSection upper-text="RECENT" bottom-text="PROJECTS">
        <div class="size-40 bg-amber-300"></div>
      </HomeSection>
      <HomeSection upper-text="12 YEARS OF" bottom-text="EXPERIENCE">
        <div class="size-40 bg-amber-300"></div>
      </HomeSection>
      <HomeSection upper-text="TECH" bottom-text="STACK">
        <div class="size-40 bg-amber-300"></div>
      </HomeSection>
    </div>
  </div>
</template>
