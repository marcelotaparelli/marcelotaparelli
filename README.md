# Marcelo Taparelli

Software Engineer focused on building reliable, secure, and performance-conscious systems while deepening my work in **AI Engineering**.

I work across backend systems, web applications, automation, product, and production environments, with a strong interest in turning real operational problems into useful, measurable software.

I’m currently pursuing a **Postgraduate Program in AI Engineering at Cruzeiro do Sul**.

## Current focus

- Software Engineering
- AI Engineering
- Backend systems and APIs
- Model evaluation and domain adaptation
- Secure Software Engineering
- Performance, observability, and production reliability
- Software architecture and automated testing
- ML Systems / AI Infrastructure — practical experimental work
- Agentic Software Development

## Core stack

**TypeScript · Bun · Node.js · Python · PyTorch · PostgreSQL · Docker**

I also work with Laravel, WordPress, CI/CD, Terraform, Redis, and cloud infrastructure.

## How I work

I prefer simple systems, explicit boundaries, and dependencies that justify their cost.

My engineering process emphasizes:

- understanding the problem before choosing technology;
- pragmatic architecture and maintainable code;
- automated tests and explicit quality gates;
- secure-by-default implementation;
- bounded resource usage and performance-aware design;
- observability and predictable failure modes;
- measurable AI evaluation instead of intuition-only decisions;
- AI coding agents with human review.

## Selected work

### ops-triage-ai

Auditable operational ticket-triage system combining a deterministic baseline, a local LLM, and a hybrid decision policy with human review, fallback, and traceability.

The project evolved into a broader AI evaluation environment covering deterministic rules, generative LLMs, and probabilistic decision models on the same frozen **70-ticket synthetic held-out benchmark**.

The original benchmark increased category accuracy from **82.9% with the deterministic baseline to 95.7% with the local LLM**, while HIGH/CRITICAL priority recall increased from **78.6% to 100%**. The deterministic baseline remained stronger on overall risk accuracy, keeping regressions and trade-offs explicit.

I later evaluated **Jev 1.13** separately on the same held-out set, where it reached **94.29% exact-tuple accuracy (66/70)** without domain-specific training from this project.

I then evaluated **Laya** zero-shot and after domain adaptation. The base checkpoint reached **11.43% exact-tuple accuracy (8/70)**; after training on **1,120 domain-specific TRAIN tickets**, validation-based checkpoint selection, and GPU training with **PyTorch/CUDA and mixed precision**, the adapted model reached **85.71% (60/70)** on the unchanged held-out set.

Jev and Laya remain **evaluation-only** and were not added to the production path or `HybridPolicy`.

The system also includes API limits, concurrency control, request IDs, structured redacted logs, metrics, health/readiness checks, graceful shutdown, and measured latency.

**Bun · TypeScript · PostgreSQL · Prisma · Ollama · Python · PyTorch · CUDA · Jev · Laya · Model Evaluation · Human-in-the-loop**

[View repository](https://github.com/marcelotaparelli/ops-triage-ai)

### resilient-transaction-api

Backend system for resilient external-payment transactions, designed around concurrent idempotency, PostgreSQL as source of truth, Redis-assisted caching and rate limiting, provider retries, circuit breaking, authentication, observability, and graceful degradation.

The project also includes Docker-based local infrastructure and a temporary AWS validation lab built with Terraform across VPC networking, ECS/Fargate, ALB, RDS, ElastiCache, ECR, Secrets Manager, IAM, and CloudWatch.

**Bun · TypeScript · PostgreSQL · Redis · Docker · Terraform · AWS · Observability · Resilience**

[View repository](https://github.com/marcelotaparelli/resilient-transaction-api)

### Salus

Backend API developed with TDD, focused on domain modeling, validation, persistence, authentication, and automated testing.

Built with strict TypeScript, Express, Prisma, and PostgreSQL. The original core was implemented manually using TDD and is evolving through hardening work focused on security, reliability, and bounded backend behavior.

**TypeScript · Node.js · Express · PostgreSQL · Prisma · TDD · Vitest**

[View repository](https://github.com/marcelotaparelli/salus)

### Professional portfolio

Bilingual engineering portfolio built with Bun, Astro, TypeScript, and MDX, with explicit quality gates for accessibility, SEO, performance, and publication integrity.

It includes CI/CD, automated artifact validation, and controlled content distribution to DEV.to and LinkedIn.

**Bun · Astro · TypeScript · MDX · Testing · Accessibility · Performance · CI/CD**

[Visit portfolio](https://marcelotaparelli.com.br)

### Google Drive → WordPress automation

Automation developed to reduce manual steps in the publishing workflow for petition pages.

**Automation · WordPress · Google Drive**

[Read the case](https://marcelotaparelli.com.br/en/projects/google-drive-wordpress/)

### Atendimento EVAG

Internal request management solution integrated with GitLab to support organization, traceability, and operational workflow.

**Software · Automation · GitLab**

[Read the case](https://marcelotaparelli.com.br/en/projects/evag-support/)

## AI Engineering

I’m extending my software engineering foundation through practical AI Engineering work involving:

- deterministic baselines and LLM integration;
- structured outputs and typed decision models;
- frozen held-out benchmarks and reproducible evaluation;
- domain adaptation and fine-tuning;
- TRAIN / VALIDATION / HELD-OUT separation;
- validation-based checkpoint selection;
- confidence and calibration analysis;
- hybrid decision systems, human review, and fallbacks;
- PyTorch, GPU/CUDA training, mixed precision, and checkpoint lifecycle;
- security, observability, latency, cost, and operational trade-offs.

My current learning and building direction includes:

- RAG and evidence-grounded systems;
- AI agents and stateful agentic workflows;
- ML Systems and AI Infrastructure;
- GPU-aware model training and inference;
- practical AWS deployment and cloud architecture.

I treat AI as an engineering tool, not as a requirement: the goal is to use it where it creates measurable value.

## Writing

I write about engineering decisions, software, AI Engineering, security, performance, reliability, and product.

Recent topics include model evaluation, Jev, Laya, domain adaptation, frozen held-outs, calibration, and the operational trade-offs of self-hosted AI.

[Read my articles](https://marcelotaparelli.com.br/en/articles/)

## Contact

- [Portfolio](https://marcelotaparelli.com.br)
- [LinkedIn](https://www.linkedin.com/in/marcelo-taparelli/)
- [Email](mailto:contato@marcelotaparelli.com.br)
