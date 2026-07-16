<template>
  <div class="flex min-h-screen flex-col bg-black text-gray-100">
    <main class="mx-auto container p-1">
      <Navigation
        class="fixed top-10 left-1/2 -translate-x-1/2 -translate-y-1/2"
      />
      <div class="mt-20.5"></div>
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
