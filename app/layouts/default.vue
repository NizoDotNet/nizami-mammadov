<template>
  <div
    class="flex min-h-screen flex-col bg-white text-gray-900 dark:bg-neutral-950 dark:text-gray-100"
  >
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
  <Navigation
    class="fixed bottom-1 left-1/2 -translate-x-1/2 -translate-y-1/2"
  />
</template>

<script setup></script>
