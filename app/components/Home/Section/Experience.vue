<script setup lang="ts">
interface Experience {
  role: string;
  company: string;
  period: string;
  bullets: string[];
}

const experience: Experience[] = [
  {
    role: "Software Engineer",
    company: "Frazex",
    period: "July 2026 to Present",
    bullets: [
      "Develop and support an omnichannel chatbot and operator platform built with a modular monolith architecture using ABP Framework.",
      "Work on a system that unifies customer conversations from WhatsApp, Telegram, Instagram, and Facebook in a single operator interface.",
      "Support a platform handling more than 100,000 messages and 20,000 support tickets per month across channels.",
      "Built a file management service using ASP.NET Core, AWS, and MinIO for chat attachments and documents.",
      "Write and optimize stored procedures and queries in SQL Server and PostgreSQL, including pagination and filtering for message and ticket retrieval.",
      "Contributed to the Mastercard Omnichannel Platform (Telegram/WhatsApp chatbot flows, routing, and support center module).",
      "Developed AZAL Omnichannel Platform conversation flows for Telegram and WhatsApp with service-based routing and Zendesk integration.",
    ],
  },
  {
    role: "Software Engineer Intern",
    company: "AzInTelecom",
    period: "February 2026 to June 2026",
    bullets: [
      "Built ASP.NET Core backend services for the ShekiSoccer platform.",
      "Developed an HTTP-header-based dynamic translation system.",
      "Built a mock payment microservice system with asynchronous RabbitMQ messaging.",
      "Integrated Keycloak for OAuth2 and OpenID Connect authentication between services.",
      "Containerized applications with Docker and configured GitLab CI/CD pipelines.",
      "Led sprint planning and technical discussions, performed code reviews, and contributed to relational schema design.",
    ],
  },
  {
    role: "Software Engineer",
    company: "Freelance",
    period: "July 2023 to December 2025",
    bullets: [
      "Delivered more than seven production platforms end to end, from client requirements and scope definition through implementation.",
      "Built a dormitory management system with asynchronous event-driven processing.",
      "Implemented CQRS, Redis caching, and SignalR real-time chat for the YouBase event platform.",
      "Built a multi-role psychological clinic CRM with service-layer data isolation.",
      "Used EF Core and Dapper together for performance-sensitive data access.",
    ],
  },
];
</script>

<template>
  <section class="bg-black">
    <div class="mx-auto max-w-6xl">
      <div class="flex flex-col">
        <article
          v-for="job in experience"
          :key="job.company + job.role"
          class="group grid grid-cols-1 gap-6 border-t border-neutral-800 py-10 sm:py-12 md:grid-cols-[280px_1fr] md:gap-12 last:border-b transition-colors duration-300 hover:bg-white/5 px-2 sm:px-4"
        >
          <div class="flex items-start gap-5">
            <div
              class="h-16 w-4 shrink-0 bg-[#FFD447] transition-transform duration-300 group-hover:scale-y-110"
            ></div>
            <div>
              <h3 class="text-2xl font-extrabold text-white md:text-3xl">
                {{ job.role }}
              </h3>
              <p class="mt-2 text-sm text-neutral-400">
                {{ job.company }}
              </p>
            </div>
          </div>

          <div class="flex flex-col gap-6">
            <ul class="flex flex-col gap-2 list-disc pl-5 text-base leading-relaxed text-neutral-300">
              <li v-for="(bullet, i) in job.bullets" :key="i">{{ bullet }}</li>
            </ul>
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
