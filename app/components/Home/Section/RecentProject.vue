<script setup lang="ts">
interface Project {
  name: string;
  tagline: string;
  description: string;
  tags: string[];
  link?: string;
}

const projects: Project[] = [
  {
    name: "Azal Omnichannel",
    tagline: "Unified support platform for AZAL Miles concierge users",
    description:
      "Centralized system consolidating customer requests from WhatsApp, Telegram, Facebook and web widgets into a single support hub. Currently integrating Zendesk for 24/7 coverage, with our team owning dedicated concierge-level support.",
    tags: ["C#", "ASP.NET", "PostgreSQL", "Zendesk API"],
  },
  {
    name: "Mastercard Concierge",
    tagline: "Multi-channel support system for Mastercard concierge services",
    description:
      "A parallel build to the AZAL project for Mastercard cardholders. Integrates a third-party platform for concierge escalations, while our team owns round-the-clock frontline support across every channel.",
    tags: ["C#", "ASP.NET", "SQL Server"],
  },
  {
    name: "Sano CRM",
    tagline: "Patient intake and doctor assignment system",
    description:
      "A CRM built for a psychological care center to streamline patient onboarding — capturing intake requests and automatically routing patients to the right doctor by availability and specialty.",
    tags: ["Vue", "CRM"],
  },
];
</script>

<template>
  <section class="bg-black">
    <div class="mx-auto max-w-6xl">
      <div class="flex flex-col">
        <article
          v-for="project in projects"
          :key="project.name"
          class="group grid grid-cols-1 gap-6 border-t border-neutral-800 py-10 md:grid-cols-[280px_1fr] md:gap-12 last:border-b"
        >
          <!-- Left: accent block + name -->
          <div class="flex items-start gap-5">
            <div
              class="h-16 w-4 shrink-0 bg-[#FFD447] transition-transform duration-300 group-hover:scale-y-110"
            />
            <div>
              <h3 class="text-2xl font-extrabold text-white md:text-3xl">
                {{ project.name }}
              </h3>
              <p class="mt-2 text-sm text-neutral-400">
                {{ project.tagline }}
              </p>
            </div>
          </div>

          <!-- Right: description + tags -->
          <div class="flex flex-col justify-between gap-6">
            <p class="text-base leading-relaxed text-neutral-300">
              {{ project.description }}
            </p>

            <div class="flex flex-wrap gap-2">
              <span
                v-for="tag in project.tags"
                :key="tag"
                class="rounded-full border border-neutral-700 px-3 py-1 text-xs font-medium text-neutral-300"
              >
                {{ tag }}
              </span>
            </div>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>
