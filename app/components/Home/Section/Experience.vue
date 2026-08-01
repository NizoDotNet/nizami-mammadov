<script setup lang="ts">
interface Experience {
  role: string;
  company: string;
  period: string;
  type: string;
  description: string;
}

const experience: Experience[] = [
  {
    role: "Software Engineer",
    company: "Frazex",
    period: "Present",
    type: "Full-time",
    description:
      "Currently building and maintaining core product features as part of the engineering team.",
  },
  {
    role: "Software Engineer Intern",
    company: "AzInTelecom",
    period: "4 months",
    type: "Internship",
    description:
      "Gained hands-on experience working within a large-scale engineering team, contributing to real production systems.",
  },
  {
    role: "Freelance Developer",
    company: "Self-employed",
    period: "2.5 years",
    type: "Freelance",
    description:
      "Delivered custom software solutions for clients across different industries, handling everything from planning to deployment.",
  },
];
</script>

<template>
  <section class="bg-black">
    <div class="mx-auto max-w-6xl">
      <div class="flex flex-col">
        <article
          v-for="job in experience"
          :key="job.company"
          class="group grid grid-cols-1 gap-6 border-t border-neutral-800 py-10 md:grid-cols-[280px_1fr] md:gap-12 last:border-b"
        >
          <!-- Left: accent dot + role/company -->
          <div class="flex items-start gap-5">
            <div
              class="h-16 w-4 shrink-0 bg-[#FFD447] transition-transform duration-300 group-hover:scale-y-110"
            ></div>
            <div>
              <h3 class="text-2xl font-extrabold text-white md:text-3xl">
                {{ job.role }}
              </h3>
              <p class="mt-2 text-sm text-neutral-400">
                {{ job.company }} · {{ job.type }}
              </p>
            </div>
          </div>

          <!-- Right: description + period -->
          <div class="flex flex-col justify-between gap-6">
            <p class="text-base leading-relaxed text-neutral-300">
              {{ job.description }}
            </p>

            <span
              class="text-xs font-semibold uppercase tracking-wider text-neutral-500"
            >
              {{ job.period }}
            </span>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>
