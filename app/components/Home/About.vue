<script setup lang="ts"></script>

<template>
  <div
    class="flex flex-col items-center text-center lg:items-start lg:text-left"
  >
    <h1
      class="font-bold leading-[0.95] text-white text-5xl sm:text-6xl md:text-7xl xl:text-9xl"
    >
      SOFTWARE
      <span class="block font-bold text-zinc-700">ENGINEER</span>
    </h1>

    <p class="ms-1 mt-4 max-w-2xl text-zinc-300 text-base sm:text-lg leading-relaxed">
      I'm Nizami, a software engineer specializing in C# and ASP.NET Core. I build backend systems and full-stack applications, with experience in API design, relational databases, asynchronous messaging, and production deployments. I care about clean architecture, practical engineering decisions, and software that solves real business problems.
    </p>
    <!-- <div class="mt-9 flex flex-wrap md:gap-10 gap-6 justify-center lg:justify-start">
      <HomeAboutCard text="5" bottom-text="Years of experience" />
    </div> -->
    <div class="mt-14 lg:mt-28 flex flex-col gap-14 lg:gap-28">
      <div id="projects" class="animate-fade-up scroll-mt-28">
        <HomeSection upper-text="RECENT" bottom-text="PROJECTS">
          <HomeSectionRecentProject></HomeSectionRecentProject>
        </HomeSection>
      </div>
      <div class="animate-fade-up animate-delay-100 scroll-mt-28">
        <HomeSection upper-text="5 YEARS OF" bottom-text="EXPERIENCE">
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
