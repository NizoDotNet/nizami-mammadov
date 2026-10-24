<template>
  <div class="flex min-h-screen flex-col bg-black text-zinc-100">
    <main class="mx-auto w-full max-w-7xl px-0 sm:px-6 lg:px-8 pb-24 md:pb-0">
      <Navigation class="fixed bottom-3 left-1/2 -translate-x-1/2 z-50 md:top-6 md:bottom-auto" />
      <div class="pt-6 md:pt-24"></div>
      <div class="px-4 sm:px-0">
        <slot />
      </div>
    </main>

    <footer
      class="mt-16 border-t border-neutral-800 px-6 py-8 text-center text-sm text-neutral-500"
    >
      <p>
        &copy; {{ new Date().getFullYear() }} Nizami Mammadov. All rights
        reserved.
      </p>
    </footer>
  </div>
</template>

<script setup></script>
