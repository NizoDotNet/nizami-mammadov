<template>
  <div class="flex min-h-screen flex-col bg-black text-zinc-100">
    <main class="mx-auto w-full max-w-7xl px-4 sm:px-6 lg:px-8">
      <Navigation class="fixed top-6 left-1/2 -translate-x-1/2 z-50" />
      <div class="pt-20 sm:pt-24"></div>
      <slot />
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
