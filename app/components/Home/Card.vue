<script setup lang="ts">
import CardLink from "./CardLink.vue";
</script>

<template>
  <div class="relative group w-full max-w-[300px] sm:max-w-[320px] lg:max-w-[300px]">
    <svg
      class="absolute inset-0 h-full w-full rounded-3xl"
      viewBox="0 0 320 420"
      preserveAspectRatio="none"
      aria-hidden="true"
    >
      <defs>
        <linearGradient id="cardStroke" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="rgba(255,255,255,0.9)" />
          <stop offset="100%" stop-color="rgba(255,255,255,0.5)" />
        </linearGradient>
      </defs>
      <rect
        x="1"
        y="1"
        width="318"
        height="418"
        rx="24"
        ry="24"
        fill="white"
        stroke="url(#cardStroke)"
        stroke-width="1"
      />
      <path
        d="M -20 60 C 40 20, 120 10, 200 40 C 280 70, 340 40, 360 30 L 360 160 C 300 140, 220 150, 140 180 C 60 210, -10 190, -20 170 Z"
        fill="rgba(0,0,0,0.03)"
      />
      <path
        d="M -10 320 C 60 290, 150 280, 240 310 C 320 340, 380 320, 400 310 L 400 440 L -30 440 Z"
        fill="rgba(0,0,0,0.02)"
      />
    </svg>
    <div
      class="relative flex flex-col items-center text-center gap-5 px-6 py-7 sm:px-7 sm:py-8 transition-transform duration-300 group-hover:-translate-y-1"
    >
      <div>
        <img
          class="object-cover rounded-2xl w-[230px] h-[185px] sm:w-[250px] sm:h-[200px]"
          src="~/assets/imgs/my-photo.JPG"
          alt="Nizami Mammadov"
        />
      </div>
      <div class="flex flex-col items-center gap-2">
        <h1 class="font-bold text-black text-2xl sm:text-3xl tracking-tight">
          Nizami Mammadov
        </h1>
        <p class="max-w-[250px] text-sm leading-relaxed text-zinc-600">
          Software Engineer crafting clean, intuitive experiences across web and
          product.
        </p>
      </div>
      <div class="flex gap-3 items-center justify-center">
        <CardLink
          link="https://github.com/nizodotnet"
          icon="i-line-md-github"
        />
        <CardLink
          link="https://www.linkedin.com/in/nizamimamedov01/"
          icon="i-ant-design-linkedin-outlined"
        />
      </div>
    </div>
  </div>
</template>
