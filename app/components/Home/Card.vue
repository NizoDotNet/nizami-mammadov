<script setup lang="ts">
import CardLink from "./CardLink.vue";
</script>

<template>
  <div
    class="bg-white flex flex-col justify-center items-center gap-6 px-5 py-8 rounded-2xl 2xl:max-w-[344px] sm:min-w-max h-min"
  >
    <div class="">
      <img
        class="object-cover rounded-2xl lg:w-50 lg:h-70 w-[260px] h-[210px]"
        src="~/assets/imgs/my-photo.JPG"
        alt=""
      />
    </div>
    <div class="flex flex-col text-center items-center">
      <div class="mt-4 xl:mb-[100px] lg:mb-[17px]">
        <h1 class="font-bold text-black text-4xl">Nizami Mammadov</h1>
      </div>
      <div class="w-[300px] lg:mb-[30px] md:mb-[20px] mb-4">
        <p class="text-center text-gray-500">
          I am super puper engineer. Lalalala i want u to love me. ALlalalal I
          want to live
        </p>
      </div>
      <div class="flex gap-4 items-center justify-center">
        <CardLink
          link="https://www.linkedin.com/in/nizamimamedov01/"
          icon="i-line-md-github"
        />
        <CardLink
          link="https://github.com/nizodotnet"
          icon="i-ant-design-linkedin-outlined"
        />
      </div>
    </div>
  </div>
</template>
