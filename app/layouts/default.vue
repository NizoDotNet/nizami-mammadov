<template>
  <div
    class="flex min-h-screen flex-col bg-white text-gray-900 dark:bg-neutral-950 dark:text-gray-100"
  >
    <header
      class="flex items-center justify-between border-b border-gray-200 px-6 py-5 dark:border-neutral-800 sm:px-8"
    >
      <NuxtLink to="/" class="text-lg font-bold tracking-tight">
        Nizami Mammadov
      </NuxtLink>

      <nav class="flex gap-6 text-sm">
        <NuxtLink
          to="/"
          class="opacity-70 transition-opacity hover:opacity-100"
          active-class="opacity-100 font-medium"
        >
          Home
        </NuxtLink>
        <NuxtLink
          to="/about"
          class="opacity-70 transition-opacity hover:opacity-100"
          active-class="opacity-100 font-medium"
        >
          About
        </NuxtLink>
        <NuxtLink
          to="/projects"
          class="opacity-70 transition-opacity hover:opacity-100"
          active-class="opacity-100 font-medium"
        >
          Projects
        </NuxtLink>
        <NuxtLink
          to="/contact"
          class="opacity-70 transition-opacity hover:opacity-100"
          active-class="opacity-100 font-medium"
        >
          Contact
        </NuxtLink>
      </nav>
    </header>

    <main class="mx-auto w-full max-w-3xl flex-1 px-6 py-12 sm:px-8">
      <slot />
    </main>

    <footer
      class="border-t border-gray-200 px-6 py-6 text-center text-sm opacity-60 dark:border-neutral-800"
    >
      <p>
        &copy; {{ new Date().getFullYear() }} Nizami Mammadov. All rights
        reserved.
      </p>
    </footer>
  </div>
</template>

<script setup></script>
