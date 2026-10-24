<script setup lang="ts"></script>

<template>
  <div
    class="flex flex-col items-center text-center lg:items-start lg:text-left"
  >
    <h1
      class="font-bold leading-[0.95] text-white text-5xl sm:text-6xl md:text-7xl xl:text-9xl"
    >
      SOFTWARE
      <span class="block font-bold text-zinc-700"> ENGINEER </span>
    </h1>

    <h4 class="ms-1 mt-4 max-w-md text-zinc-400 text-sm sm:text-base">
      Passionate about creating intuitive and engaging user experiences.
      Specialize in transforming ideas into beautifully crafted products.
    </h4>
    <div class="mt-9 flex flex-wrap md:gap-10 gap-6 justify-center lg:justify-start">
      <HomeAboutCard text="+12" bottom-text="Years of experience" />
      <HomeAboutCard text="+45" bottom-text="Projects completed" />
      <HomeAboutCard text="+40" bottom-text="World Wide Clients" />
    </div>
    <div class="mt-14 lg:mt-28 flex flex-col gap-14 lg:gap-28">
      <div id="projects" class="animate-fade-up scroll-mt-28">
        <HomeSection upper-text="RECENT" bottom-text="PROJECTS">
          <HomeSectionRecentProject></HomeSectionRecentProject>
        </HomeSection>
      </div>
      <div class="animate-fade-up animate-delay-100 scroll-mt-28">
        <HomeSection upper-text="12 YEARS OF" bottom-text="EXPERIENCE">
          <HomeSectionExperience> </HomeSectionExperience>
        </HomeSection>
      </div>
      <div id="tools" class="animate-fade-up animate-delay-200 scroll-mt-28">
        <HomeSection upper-text="TECH" bottom-text="STACK">
          <HomeSectionTechStack></HomeSectionTechStack>
        </HomeSection>
      </div>
      <div id="blog" class="scroll-mt-28"></div>
    </div>
  </div>
</template>
