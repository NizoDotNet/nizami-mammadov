# Nizami Mammadov | Software Engineer

Software engineer specializing in C# and ASP.NET Core. I build backend systems and full-stack applications with experience in API design, relational databases, asynchronous messaging, and production deployments. I care about clean architecture, practical engineering decisions, and software that solves real business problems.

## About

I'm Nizami, a software engineer with 5 years of experience. Focused on C# and ASP.NET Core, backend systems, and full-stack applications.

## Experience

### Software Engineer, Frazex
*July 2026 to Present*

- Develop and support an omnichannel chatbot and operator platform built with a modular monolith architecture using ABP Framework.
- Work on a system that unifies customer conversations from WhatsApp, Telegram, Instagram, and Facebook in a single operator interface.
- Support a platform handling more than 100,000 messages and 20,000 support tickets per month across channels.
- Built a file management service using ASP.NET Core, AWS, and MinIO for chat attachments and documents.
- Write and optimize stored procedures and queries in SQL Server and PostgreSQL, including pagination and filtering for message and ticket retrieval.
- Contributed to the Mastercard Omnichannel Platform (Telegram/WhatsApp chatbot flows, routing, and support center module).
- Developed AZAL Omnichannel Platform conversation flows for Telegram and WhatsApp with service-based routing and Zendesk integration.

### Software Engineer Intern, AzInTelecom
*February 2026 to June 2026*

- Built ASP.NET Core backend services for the ShekiSoccer platform.
- Developed an HTTP-header-based dynamic translation system.
- Built a mock payment microservice system with asynchronous RabbitMQ messaging.
- Integrated Keycloak for OAuth2 and OpenID Connect authentication between services.
- Containerized applications with Docker and configured GitLab CI/CD pipelines.
- Led sprint planning and technical discussions, performed code reviews, and contributed to relational schema design.

### Software Engineer, Freelance
*July 2023 to December 2025*

- Delivered more than seven production platforms end to end, from client requirements and scope definition through implementation.
- Built a dormitory management system with asynchronous event-driven processing.
- Implemented CQRS, Redis caching, and SignalR real-time chat for the YouBase event platform.
- Built a multi-role psychological clinic CRM with service-layer data isolation.
- Used EF Core and Dapper together for performance-sensitive data access.

## Recent Projects

### Mastercard Omnichannel Platform
Developed an omnichannel chatbot platform that handles customer requests through Telegram and WhatsApp, manages conversational flows, and routes customers to the appropriate support channels. The platform includes a support center module that directs customer conversations to human operators when assistance is required.

*Technologies:* C#, PostgreSQL, Docker, CI/CD, IIS

### AZAL Omnichannel Platform
Developed omnichannel conversation flows for Telegram and WhatsApp, with service-based routing. Integrated Zendesk to forward messages to the appropriate support team when customers select 24/7 support. Requests from customers selecting the concierge service are routed to the internal support team instead.

*Technologies:* C#, PostgreSQL, Docker, CI/CD

### Mock Payment Microservice System
A standalone payment system built to model production payment workflows. It separates order, payment, and notification flows using asynchronous RabbitMQ messaging. It uses Keycloak for service-to-service OAuth2/OpenID Connect authentication, with Docker and GitLab CI/CD for deployment workflows.

*Technologies:* C#, ASP.NET Core, RabbitMQ, Keycloak, SQL Server, Docker, GitLab CI/CD

### YouBase Event Platform
An event platform built with ASP.NET Core and Vue.js. The project uses CQRS with MediatR to separate read and write operations, Redis for caching, and SignalR for real-time chat.

*Technologies:* ASP.NET Core, C#, Vue.js, MediatR, Redis, SignalR

### Dormitory Management System
A system designed to automate multi-step dormitory workflows and student registrations. The system handled more than 1,000 concurrent student registrations using an asynchronous RabbitMQ pipeline.

*Technologies:* C#, ASP.NET Core, RabbitMQ

### ShekiSoccer Platform
A football platform for more than 1,000 active fans. Backend work included an HTTP-header-based dynamic translation system to reduce client-side localization overhead.

*Technologies:* ASP.NET Core, C#

## Tech Stack

### Backend
- C#
- .NET
- ASP.NET Core
- REST APIs
- Entity Framework Core
- Dapper
- LINQ

### Architecture and Messaging
- Clean Architecture
- Modular Monolith
- Microservices
- CQRS with MediatR
- RabbitMQ
- SignalR
- Redis

### Databases and Infrastructure
- PostgreSQL
- SQL Server
- AWS
- MinIO
- Docker
- GitLab CI/CD
- Git
- IIS

### Frontend
- JavaScript
- TypeScript
- Vue.js
- Angular
- ASP.NET MVC

## Portfolio
This repository contains the source code for my personal portfolio website built with Nuxt 4, Vue 3, and Tailwind CSS.
