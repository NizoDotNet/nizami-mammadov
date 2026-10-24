<script setup lang="ts">
import CardLink from "./CardLink.vue";
</script>

<template>
  <div class="relative group w-full max-w-[320px] sm:max-w-[340px] lg:max-w-[320px]">
    <div
      class="absolute -inset-[1px] rounded-3xl bg-gradient-to-br from-white/40 via-white/10 to-transparent opacity-70 blur-[0.5px] transition-opacity duration-500 group-hover:opacity-100"
    ></div>
    <div
      class="relative flex flex-col items-center text-center gap-5 px-6 py-7 sm:px-7 sm:py-8 rounded-3xl bg-gradient-to-b from-white/[0.12] to-white/[0.04] backdrop-blur-xl border border-white/10 shadow-[0_60px_120px_-80px_rgba(255,255,255,0.5)] transition-transform duration-500 group-hover:-translate-y-1"
    >
      <div class="relative">
        <div
          class="absolute -inset-1 rounded-2xl bg-gradient-to-br from-white/30 to-white/0 blur-lg opacity-60 group-hover:opacity-90 transition-opacity duration-500"
        ></div>
        <img
          class="relative object-cover rounded-2xl w-[240px] h-[190px] sm:w-[260px] sm:h-[210px]"
          src="~/assets/imgs/my-photo.JPG"
          alt="Nizami Mammadov"
        />
      </div>
      <div class="flex flex-col items-center gap-3">
        <h1 class="font-bold text-white text-2xl sm:text-3xl tracking-tight">
          Nizami Mammadov
        </h1>
        <p class="max-w-[260px] text-sm leading-relaxed text-zinc-300">
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
