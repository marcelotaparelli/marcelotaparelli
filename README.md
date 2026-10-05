# Marcelo Taparelli

**AI Engineer & Software Engineer | Python, RAG, Agents, Evals | TypeScript, Bun | Product-minded**

I build reliable AI products and backend systems from problem to production.

My work combines **AI Engineering** — RAG, agentic workflows, evaluation, guardrails and observability — with **Software Engineering** in TypeScript/Bun, PostgreSQL, Redis, Docker and cloud infrastructure.

I care about the product problem first: measurable outcomes, explicit trade-offs, security, reliability and systems that can actually be operated in production.

I’m currently pursuing a **Postgraduate Program in AI Engineering**.

## Current focus

- AI Engineering
- RAG and evidence-grounded systems
- AI Agents and agentic workflows
- LLM evaluation and guardrails
- Backend systems and APIs
- Secure Software Engineering
- Observability and production reliability
- Model evaluation and domain adaptation
- ML Systems / AI Infrastructure
- Product Engineering

## Core stack

### AI Engineering

**Python · FastAPI · RAG · Embeddings · pgvector · Agents · LangGraph · OpenAI · Evals · PyTorch · OpenTelemetry**

### Software Engineering

**TypeScript · Bun · Node.js · PostgreSQL · Redis · Docker · Terraform · AWS**

### Product Engineering

**Product thinking · Architecture · Security · Performance · Observability · Automated testing · CI/CD**

I also work with Prisma, Express, Astro, Laravel, WordPress and cloud infrastructure.

## How I work

I prefer simple systems, explicit boundaries and dependencies that justify their cost.

My engineering process emphasizes:

- understanding the product problem before choosing technology;
- pragmatic architecture and maintainable code;
- deterministic controls around probabilistic AI systems;
- automated tests and explicit quality gates;
- secure-by-default implementation;
- bounded resource usage and performance-aware design;
- observability and predictable failure modes;
- measurable AI evaluation instead of intuition-only decisions;
- human approval around high-impact AI actions;
- explicit trade-offs between quality, latency, cost and reliability.

## Selected work

### OpsPilot AI

Production-oriented AI operations copilot built around **evidence-grounded RAG and approval-gated agentic workflows**.

The system combines hybrid retrieval with PostgreSQL/pgvector, bounded LangGraph orchestration, structured outputs, human approval before external actions, OpenAI integration, real GitLab execution, evaluation gates, OpenTelemetry observability and security guardrails.

The architecture includes tenant isolation with PostgreSQL RLS, deterministic policy enforcement outside the LLM, immutable action hashes, idempotent external actions, reconciliation for ambiguous provider outcomes, citation validation, structured logging and fail-open telemetry.

The project also includes real post-release integration evidence against **OpenAI and GitLab**, automated regression gates, security testing and CI/CD release validation.

**Python · FastAPI · RAG · pgvector · LangGraph · OpenAI · GitLab · PostgreSQL · OpenTelemetry · Docker · Terraform**

[View repository](https://github.com/marcelotaparelli/opspilot-ai)

### ops-triage-ai

Auditable operational ticket-triage system combining a deterministic baseline, a local LLM and a hybrid decision policy with human review, fallback and traceability.

The project evolved into an AI evaluation environment covering deterministic rules, generative LLMs and probabilistic decision models on the same frozen **70-ticket synthetic held-out benchmark**.

The original benchmark increased category accuracy from **82.9% with the deterministic baseline to 95.7% with the local LLM**, while HIGH/CRITICAL priority recall increased from **78.6% to 100%**. The deterministic baseline remained stronger on overall risk accuracy, keeping regressions and trade-offs explicit.

I later evaluated **Jev 1.13** separately on the same held-out set, where it reached **94.29% exact-tuple accuracy (66/70)** without domain-specific training from this project.

I also evaluated **Laya** zero-shot and after domain adaptation. The base checkpoint reached **11.43% exact-tuple accuracy (8/70)**; after training on **1,120 domain-specific TRAIN tickets**, validation-based checkpoint selection and GPU training with **PyTorch/CUDA and mixed precision**, the adapted model reached **85.71% (60/70)** on the unchanged held-out set.

Jev and Laya remain **evaluation-only** and were not added to the production path or `HybridPolicy`.

The system also includes API limits, concurrency control, request IDs, structured redacted logs, metrics, health/readiness checks, graceful shutdown and measured latency.

**Bun · TypeScript · PostgreSQL · Prisma · Ollama · Python · PyTorch · CUDA · Jev · Laya · Model Evaluation · Human-in-the-loop**

[View repository](https://github.com/marcelotaparelli/ops-triage-ai)

### resilient-transaction-api

Backend system for resilient external-payment transactions, designed around concurrent idempotency, PostgreSQL as source of truth, Redis-assisted caching and rate limiting, provider retries, circuit breaking, authentication, observability and graceful degradation.

The project includes Docker-based local infrastructure and an AWS validation lab built with Terraform across VPC networking, ECS/Fargate, ALB, RDS, ElastiCache, ECR, Secrets Manager, IAM and CloudWatch.

It focuses on the kind of reliability concerns that become especially important when AI systems depend on external providers, asynchronous workflows and distributed infrastructure.

**Bun · TypeScript · PostgreSQL · Redis · Docker · Terraform · AWS · Observability · Resilience**

[View repository](https://github.com/marcelotaparelli/resilient-transaction-api)

### Salus

Backend API developed with TDD, focused on domain modeling, validation, persistence, authentication and automated testing.

Built with strict TypeScript, Express, Prisma and PostgreSQL. The project explores clean architecture, use-case boundaries, ownership, security and maintainable backend design.

**TypeScript · Node.js · Express · PostgreSQL · Prisma · TDD · Vitest**

[View repository](https://github.com/marcelotaparelli/salus)

### Professional portfolio

Bilingual engineering portfolio built with Bun, Astro, TypeScript and MDX, with explicit quality gates for accessibility, SEO, performance and publication integrity.

It includes CI/CD, automated artifact validation and controlled content distribution.

**Bun · Astro · TypeScript · MDX · Testing · Accessibility · Performance · CI/CD**

[Visit portfolio](https://marcelotaparelli.com.br)

### Google Drive → WordPress automation

Automation developed to reduce manual steps in the publishing workflow for petition pages.

**Automation · WordPress · Google Drive**

[Read the case](https://marcelotaparelli.com.br/en/projects/google-drive-wordpress/)

### Atendimento EVAG

Internal request management solution integrated with GitLab to support organization, traceability and operational workflow.

**Software · Automation · GitLab**

[Read the case](https://marcelotaparelli.com.br/en/projects/evag-support/)

## AI Engineering

I build and evaluate AI systems with the same engineering discipline I apply to backend software.

My work includes:

- RAG and evidence-grounded generation;
- embeddings and vector search with pgvector;
- agentic workflows with bounded tool use;
- human approval before high-impact external actions;
- structured outputs and typed contracts;
- deterministic policy enforcement around probabilistic models;
- offline and live evaluation;
- frozen held-out datasets and reproducible benchmarks;
- deterministic baselines for comparison;
- domain adaptation and fine-tuning;
- TRAIN / VALIDATION / HELD-OUT separation;
- validation-based checkpoint selection;
- confidence and calibration analysis;
- observability for LLM, retrieval and agent workflows;
- latency, security and cost controls;
- failure handling, fallbacks and reconciliation;
- PyTorch, GPU/CUDA training and mixed precision.

I treat AI as a component inside a larger software system.

The model may be probabilistic; the surrounding system should provide **schemas, policies, tests, metrics, observability, security boundaries, fallbacks and human control**.

## Product Engineering

I’m interested in the intersection of **AI, software engineering and product**.

That means starting from a real problem, understanding the operational constraints and then choosing the simplest architecture capable of delivering measurable value.

For me, engineering is not only about making software work. It is also about deciding:

- whether AI is actually necessary;
- what should remain deterministic;
- what failures are acceptable;
- what needs human approval;
- what should be measured;
- how the system behaves under degraded conditions;
- whether the complexity creates enough product value to justify its cost.

## Writing

I write about AI Engineering, software architecture, model evaluation, agentic systems, security, performance, reliability and product engineering.

Recent topics include model evaluation, Jev, Laya, domain adaptation, frozen held-outs, calibration and the operational trade-offs of self-hosted AI.

[Read my articles](https://marcelotaparelli.com.br/en/articles/)

## Contact

- [Portfolio](https://marcelotaparelli.com.br)
- [LinkedIn](https://www.linkedin.com/in/marcelo-taparelli/)
- [GitHub](https://github.com/marcelotaparelli)
- [Email](mailto:contato@marcelotaparelli.com.br)
