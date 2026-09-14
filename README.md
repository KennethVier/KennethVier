<div align="center">

![Kenneth Vier — Software Engineer](./assets/profile-hero.svg)

[![Portfolio](https://img.shields.io/badge/Portfolio-vier--main--portfolio.vercel.app-111827?style=for-the-badge&logo=vercel&logoColor=white)](https://vier-main-portfolio.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-KennethVier-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KennethVier)

</div>

## Engineering Profile

I'm a **Software Engineer** focused on backend-heavy full-stack systems with **Java, Spring Boot, React, PostgreSQL, and AI integration**.

I care about the parts of software that tend to matter after the demo works: **clear architecture, transactional correctness, concurrency, validation, migrations, testability, security boundaries, observability, and maintainability**.

My current direction sits at the intersection of traditional software engineering and AI engineering—building systems where LLMs are bounded components rather than the architecture itself.

```text
Product problem
    ↓
Domain + architecture
    ↓
Reliable backend / data boundaries
    ↓
AI where it adds leverage
    ↓
Validation, testing, observability
```

---

## Featured Engineering Projects

### 🧠 [Hippocampus](https://github.com/KennethVier/hippocampus)

**Medical learning platform built around evidence-grounded Study Missions.**

Hippocampus is my most architecture-intensive project. Its v1 design uses a **modular monolith**, bounded AI provider integrations, a **database-backed background worker model**, and a retrieval layer designed to keep learning output grounded and traceable to source material.

**Architecture & engineering highlights**

- **Java 25 + Spring Boot 4.1 + Spring Framework 7** modular backend
- Spring MVC REST APIs with **SSE** where streaming is appropriate
- **Spring Security + server-side sessions + Spring Session JDBC**
- **Spring Data JPA / Hibernate** with PostgreSQL and explicit transaction boundaries
- **PostgreSQL 18 + pgvector + full-text search + pg_trgm** for relational, vector, and lexical retrieval
- **Flyway** for schema evolution
- **Spring AI 2.0** with provider abstraction for Gemini and Ollama
- PDF/document ingestion through **Apache Tika + Apache PDFBox**
- Database-backed processing jobs and Spring-managed workers for asynchronous ingestion work
- **React 19 + TypeScript 6 + Vite 8 + Tailwind CSS 4** frontend
- **TanStack Query, React Router, React Hook Form, Zod** for server state, routing, and validated forms
- Testing with **JUnit 5, Mockito, AssertJ, Testcontainers, ArchUnit, Vitest, React Testing Library, and Playwright**
- Local development through **Docker Compose** with CI through **GitHub Actions**

> Engineering theme: keep AI replaceable, application state deterministic, evidence traceable, and failure modes explicit.

---

### 💸 [PesoPilot](https://peso-pilot-three.vercel.app/)

**Local-first personal finance tracker with AI-assisted financial insights.**

PesoPilot is designed around a privacy-first principle: the primary financial dataset lives locally instead of requiring an account or cloud database for normal use.

**Architecture & engineering highlights**

- **React + Vite + Tailwind CSS** application shell
- **IndexedDB + Dexie.js** as the local persistence layer
- Repository-based data access around expenses, income, savings, budgets, salary cutoffs, merchant rules, AI insights, and cash-flow snapshots
- **Zustand** for focused client state
- **React Hook Form + Zod** for schema-driven validation
- Search and combined filtering across transaction data
- **Java 21 + Spring Boot 3** service layer for backend/AI capabilities
- Local-first boundaries keep core finance workflows usable without depending on remote infrastructure

[**Open live PesoPilot demo →**](https://peso-pilot-three.vercel.app/)

> Status: actively developed and publicly deployed on Vercel.

---

### 📚 [Yomira](https://github.com/KennethVier/vier-portfolio-labs/tree/master/apps/yomira-web)

**Document-driven learning application that turns PDFs into AI-assisted learning material.**

Yomira is split into dedicated document-processing and quiz-generation services, giving each concern a clear service boundary rather than placing extraction, persistence, and LLM behavior into one application.

**Architecture & engineering highlights**

- **Java 21 + Spring Boot 3.5** backend services
- Separate **document-service** and **quiz-service** boundaries
- **Spring AI 1.1** for AI-assisted generation
- **Spring Web + WebFlux** for HTTP integration
- **Apache PDFBox** for PDF extraction
- **Spring Data JPA + PostgreSQL** for persistence
- **React 19 + Vite 7 + Axios** frontend
- Embedded PDF reading experience with React PDF tooling
- Microservice-style deployment boundaries for independent frontend/backend services

[Explore the broader Vier Portfolio Labs →](https://github.com/KennethVier/vier-portfolio-labs)

---

## Engineering Stack

### Backend & Application Architecture

<p>
  <img src="https://img.shields.io/badge/Java_25-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_Boot_4-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring_AI-6DB33F?style=flat-square&logo=spring&logoColor=white" />
  <img src="https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white" />
  <img src="https://img.shields.io/badge/REST_APIs-005571?style=flat-square" />
  <img src="https://img.shields.io/badge/SSE-0F172A?style=flat-square" />
</p>

`Spring MVC` · `Spring Security` · `Spring Data JPA` · `Hibernate` · `Spring Session JDBC` · `Bean Validation` · `WebClient/WebFlux` · `JWT/OAuth2` · `Modular Monoliths` · `Background Workers`

### Data, Persistence & Retrieval

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/pgvector-336791?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" />
  <img src="https://img.shields.io/badge/IndexedDB-111827?style=flat-square" />
  <img src="https://img.shields.io/badge/Dexie.js-8B5CF6?style=flat-square" />
</p>

`Relational modeling` · `Transactions` · `Schema migrations` · `Vector search` · `PostgreSQL FTS` · `pg_trgm` · `Repository patterns` · `Local-first persistence`

### Frontend Engineering

<p>
  <img src="https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/TypeScript_6-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Vite_8-646CFF?style=flat-square&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS_4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/TanStack_Query-FF4154?style=flat-square&logo=reactquery&logoColor=white" />
</p>

`React Router` · `React Hook Form` · `Zod` · `Zustand` · `Axios` · `Responsive UI` · `Component architecture` · `Server/client state separation`

### AI, RAG & Agentic Engineering

<p>
  <img src="https://img.shields.io/badge/Cursor-AI_Coding-111827?style=flat-square" />
  <img src="https://img.shields.io/badge/OpenAI_Codex-Agentic_Coding-000000?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG-7C3AED?style=flat-square" />
  <img src="https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache_Tika-D22128?style=flat-square&logo=apache&logoColor=white" />
  <img src="https://img.shields.io/badge/PDFBox-D22128?style=flat-square&logo=apache&logoColor=white" />
</p>

`Cursor` · `OpenAI Codex` · `AI-assisted development` · `Agentic coding workflows` · `Validation loops` · `LLM provider abstraction` · `Embeddings` · `Grounded retrieval` · `Vector + lexical search` · `Prompt engineering` · `PDF ingestion` · `Structured AI output` · `AI evaluation`

### Testing, Quality & Delivery

<p>
  <img src="https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white" />
  <img src="https://img.shields.io/badge/Testcontainers-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
</p>

`Mockito` · `AssertJ` · `ArchUnit` · `React Testing Library` · `ESLint` · `Integration testing` · `Architecture tests` · `E2E testing` · `CI validation`

### Additional Experience

`C#` · `SAP Crystal Reports` · `Thymeleaf` · `DBFlute` · `MySQL` · `SQL Server` · `Bootstrap` · `Sass` · `jQuery` · `Postman`

---

## What I'm Exploring Now

```java
public record EngineeringDirection(
        String backend,
        String ai,
        String quality,
        String goal
) {}

var currentFocus = new EngineeringDirection(
        "Reliable Java / Spring systems",
        "RAG, AI integration, and agentic workflows",
        "Validation, testing, security, and observability",
        "AI-enabled software that remains maintainable without the AI"
);
```

I'm particularly interested in **AI-assisted engineering workflows with Cursor and Codex**, **agentic systems with validation loops**, and integrating AI into Spring applications without giving up deterministic application boundaries.

---

## GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=KennethVier&show_icons=true&hide_border=true&rank_icon=github&include_all_commits=true&theme=transparent" alt="Kenneth Vier's GitHub stats" />

</div>

---

<div align="center">

### Build useful systems. Keep the boundaries clear. Validate what matters.

[**Portfolio**](https://vier-main-portfolio.vercel.app) · [**Hippocampus**](https://github.com/KennethVier/hippocampus) · [**PesoPilot**](https://peso-pilot-three.vercel.app/) · [**Portfolio Labs**](https://github.com/KennethVier/vier-portfolio-labs) · [**Repositories**](https://github.com/KennethVier?tab=repositories)

</div>
