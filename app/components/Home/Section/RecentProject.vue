<script setup lang="ts">
interface Project {
  name: string;
  description: string;
  tags: string[];
  link?: string;
}

const projects: Project[] = [
  {
    name: "Mastercard Omnichannel Platform",
    description:
      "Developed an omnichannel chatbot platform that handles customer requests through Telegram and WhatsApp, manages conversational flows, and routes customers to the appropriate support channels. The platform includes a support center module that directs customer conversations to human operators when assistance is required.",
    tags: ["C#", "PostgreSQL", "Docker", "CI/CD", "IIS"],
  },
  {
    name: "AZAL Omnichannel Platform",
    description:
      "Developed omnichannel conversation flows for Telegram and WhatsApp, with service-based routing. Integrated Zendesk to forward messages to the appropriate support team when customers select 24/7 support. Requests from customers selecting the concierge service are routed to the internal support team instead.",
    tags: ["C#", "PostgreSQL", "Docker", "CI/CD"],
  },
  {
    name: "Mock Payment Microservice System",
    description:
      "A standalone payment system built to model production payment workflows. It separates order, payment, and notification flows using asynchronous RabbitMQ messaging. It uses Keycloak for service-to-service OAuth2/OpenID Connect authentication, with Docker and GitLab CI/CD for deployment workflows.",
    tags: ["C#", "ASP.NET Core", "RabbitMQ", "Keycloak", "SQL Server", "Docker", "GitLab CI/CD"],
  },
  {
    name: "YouBase Event Platform",
    description:
      "An event platform built with ASP.NET Core and Vue.js. The project uses CQRS with MediatR to separate read and write operations, Redis for caching, and SignalR for real-time chat.",
    tags: ["ASP.NET Core", "C#", "Vue.js", "MediatR", "Redis", "SignalR"],
  },
  {
    name: "Dormitory Management System",
    description:
      "A system designed to automate multi-step dormitory workflows and student registrations. The system handled more than 1,000 concurrent student registrations using an asynchronous RabbitMQ pipeline.",
    tags: ["C#", "ASP.NET Core", "RabbitMQ"],
  },
  {
    name: "ShekiSoccer Platform",
    description:
      "A football platform for more than 1,000 active fans. Backend work included an HTTP-header-based dynamic translation system to reduce client-side localization overhead.",
    tags: ["ASP.NET Core", "C#"],
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
          class="group grid grid-cols-1 gap-6 border-t border-neutral-800 py-10 sm:py-12 md:grid-cols-[280px_1fr] md:gap-12 last:border-b transition-colors duration-300 hover:bg-white/5 px-2 sm:px-4"
        >
          <div class="flex items-start gap-5">
            <div
              class="h-16 w-4 shrink-0 bg-[#FFD447] transition-transform duration-300 group-hover:scale-y-110"
            ></div>
            <div>
              <h3 class="text-2xl font-extrabold text-white md:text-3xl">
                {{ project.name }}
              </h3>
            </div>
          </div>

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
