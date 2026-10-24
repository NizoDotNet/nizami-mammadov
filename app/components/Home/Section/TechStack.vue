<script setup lang="ts">
interface StackGroup {
  label: string;
  items: string[];
}

const stack: StackGroup[] = [
  {
    label: "Backend",
    items: ["C#", ".NET", "ASP.NET Core", "REST APIs", "Entity Framework Core", "Dapper", "LINQ"],
  },
  {
    label: "Architecture and messaging",
    items: ["Clean Architecture", "Modular Monolith", "Microservices", "CQRS with MediatR", "RabbitMQ", "SignalR", "Redis"],
  },
  {
    label: "Databases and infrastructure",
    items: ["PostgreSQL", "SQL Server", "AWS", "MinIO", "Docker", "GitLab CI/CD", "Git"],
  },
  {
    label: "Frontend",
    items: ["JavaScript", "TypeScript", "Vue.js", "Angular", "ASP.NET MVC"],
  },
];
</script>

<template>
  <section class="bg-black">
    <div class="mx-auto max-w-6xl">
      <div class="flex flex-col">
        <div
          v-for="group in stack"
          :key="group.label"
          class="group grid grid-cols-1 gap-6 border-t border-neutral-800 py-10 sm:py-12 md:grid-cols-[280px_1fr] md:gap-12 last:border-b transition-colors duration-300 hover:bg-white/5 px-2 sm:px-4"
        >
          <!-- Left: accent bar + group label -->
          <div class="flex items-start gap-5">
            <div
              class="h-16 w-4 shrink-0 bg-[#FFD447] transition-transform duration-300 group-hover:scale-y-110"
            ></div>
            <h3 class="text-2xl font-extrabold text-white md:text-3xl">
              {{ group.label }}
            </h3>
          </div>

          <!-- Right: tech items -->
          <div class="flex flex-wrap gap-3">
            <span
              v-for="item in group.items"
              :key="item"
              class="rounded-full border border-neutral-700 px-4 py-2 text-sm font-medium text-neutral-300 transition-colors duration-300 hover:border-[#FFD447] hover:text-white"
            >
              {{ item }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
