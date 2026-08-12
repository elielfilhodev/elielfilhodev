<h1 align="center">Eliel</h1>

<p align="center">
  <strong>Full Stack Developer</strong> · TypeScript · Node.js · Next.js · PostgreSQL<br>
  I build e-commerce and internal systems that run in production — and I keep them running.
</p>

<p align="center">
  <a href="{{LINKEDIN_URL}}"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:{{EMAIL}}"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="{{PORTFOLIO_URL}}"><img src="https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio"></a>
</p>

---

## About

I'm a full stack developer based in Brazil, working at the intersection of **software engineering and real retail operations**. I currently run e-commerce for a mobile phone retail chain — which means I don't just ship features, I live with the consequences: broken checkouts, fiscal compliance, inventory drift, support tickets at 9pm.

That perspective shapes how I build. I favour **boring, maintainable architecture** over clever abstractions, and I design for the failure cases first — offline machines, payment gateways timing out, tax rules that change next quarter.

- 🛒 Domain focus: **e-commerce, payments, and back-office systems**
- 🌍 Open to **remote (EU/US timezones)** and **relocation to Europe**
- 🗣️ Portuguese (native) · English (professional working proficiency)

---

## Selected Work

### 🛍️ Top Cell — E-commerce Platform
Modular monolith for a mobile phone retail chain: customer storefront, back-office, and a domain API.

**Stack:** Next.js · Clerk · shadcn/ui · Java (Spring Boot) · PostgreSQL · Redis · Flyway
**Why it's built this way:** a modular monolith gave clear domain boundaries without the operational cost of microservices for a single-team project. Payment providers (Pagar.me / Mercado Pago) and fiscal document emission sit behind interfaces, so swapping a provider is a module change — not a rewrite.

→ [Repository]({{REPO_TOPCELL}})

---

### 🎵 meucarinho.com.br — AI Music Generation Platform
Solo-shipped product: personalised AI-generated songs, from landing page to payment to delivery.

**Stack:** Next.js · Node.js · PostgreSQL · payment integration · custom back-office
**Why it matters:** end-to-end ownership — pricing, checkout flow, async generation pipeline, admin tooling, and post-sale support. Shipping alone forces ruthless scope decisions.

→ [Live site](https://meucarinho.com.br) · [Repository]({{REPO_MEUCARINHO}})

---

### 🧾 Offline-First POS — Local Point of Sale
Point-of-sale system for a small food business, designed to work with **zero internet dependency**.

**Stack:** Next.js · Fastify · TypeScript · SQLite (Prisma) · ESC/POS thermal printing
**Key decision:** the whole system runs on a single machine, because a snack shop can't stop selling when the connection drops. Fiscal document emission is abstracted behind an `EmissorDocumento` interface, so NFC-e compliance becomes a modular swap instead of a refactor.

→ [Repository]({{REPO_POS}})

---

### 🏥 Clinic Scheduling System
Appointment platform with role-based access (Admin, Doctor, Receptionist).

**Stack:** Next.js (App Router) · Prisma · NeonDB · NextAuth
**Why it's built this way:** authorisation enforced server-side per role, not hidden in the UI — the most common access-control mistake in scheduling apps.

→ [Repository]({{REPO_CLINIC}})

---

## Tech I Actually Use

**Languages**
`TypeScript` `JavaScript` `Java` `SQL`

**Frontend**
`Next.js` `React` `Tailwind CSS` `shadcn/ui`

**Backend**
`Node.js` `Fastify` `Spring Boot` `Prisma` `Zod` `REST APIs`

**Data**
`PostgreSQL` `SQLite` `Redis` `Flyway`

**Tooling & Ops**
`Docker` `Git` `GitHub Actions` `Vitest` `Linux (Ubuntu)` `Vercel`

> I list what I've shipped with, not what I've read about. Happy to learn the rest on the job.

---

## Currently

- Building a **production-grade Fastify + TypeScript backend** with layered architecture, Zod validation, Vitest coverage and CI on GitHub Actions — as a reference implementation, not a toy project.
- Deepening **Civil Engineering** fundamentals, with a long-term interest in **construtech / BIM automation** (Revit API, IFC pipelines) — where structured domain knowledge meets software.

---

## Let's Talk

If you're hiring for **frontend or full stack roles in e-commerce, fintech-adjacent products, or internal tooling**, I'd be glad to talk.

📫 **{{EMAIL}}** · 💼 **[LinkedIn]({{LINKEDIN_URL}})**
