<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1200&color=20C20E&center=true&vCenter=true&width=520&lines=wake+up%2C+visitor...;full+stack+%C2%B7+AI+engineering+%C2%B7+technical+SEO;follow+the+white+rabbit." alt="wake up, visitor..." />
</div>

### Armando Monteiro

**Full Stack Developer · TypeScript and Python · in production since 2024**

Sole developer at a performance marketing agency since December 2025. I own the architecture, the Google Cloud infrastructure and the CI/CD of three internal products, and I ship LLM features that have to survive real client data.

Rio de Janeiro, Brazil (UTC−3) · English C1

---

### Selected work

Private repositories, so here is what they do and how.

**LLM agent that explains a client's traffic change.** It gets two Google Search Console tools and decides which to call and with what parameters: when it suspects seasonality, it pulls 16 months of history on its own. Output is schema-validated field by field, and any failed step falls back to a deterministic diagnosis instead of breaking the report.
→ monthly report from **1.5–2 h to ~30 min**

**Figma to page builder generator, in Python.** Reads the design tree through the Figma REST API and emits native page builder components with LLM assistance. The LLM is grounded on a field dictionary extracted from the platform itself, so an invented field fails the build instead of being silently dropped on the client's site weeks later.
→ **~8 h to ~2 h per page**

**Live site audit API, used at event booths.** Eight independent analyses (robots.txt per crawler, rendering, structured data, Core Web Vitals field vs. lab, SERP position). A failing analysis returns its own status and never takes the report down. It fetches URLs typed by strangers, so SSRF protection has its own test suite gating every release.

**Google Cloud from zero.** Cloud Run, Cloud SQL, Secret Manager, Artifact Registry. Migrations run before the new revision serves traffic, deploys are keyless through Workload Identity Federation, and the build fails if a credential lands in the client bundle.

**WordPress component plugin.** 60 components, 1,400+ editor controls, **651 production deploys**. Custom linters enforce project invariants, and each component carries its performance budget: LCP image with high priority and no lazy loading, explicit dimensions against CLS, CSS loaded per component.

---

### Learning in public: retrieval with evaluation

Hybrid search over my own notes (~900 sections): a lexical baseline plus local embeddings through Ollama, fused with Reciprocal Rank Fusion. It is measured against 29 hand-written questions with known answers.

| Mode | recall@5 |
|---|---|
| lexical baseline | 79% |
| hybrid | **90%** |

The rule, written before any number existed: nothing ships unless it beats the baseline. Vector search alone lost to the baseline at rank 1, so it didn't ship. Hybrid did. Two embedding models tied at 26/29, so the cheaper one stayed.

---

### Public code

| Project | What it shows |
|---|---|
| [SEO Helper](https://github.com/armandomonteir-o/seo-helper-cli) | Python CLI, Command Pattern, 91% coverage |
| [Intelligent Prompt Generator](https://github.com/armandomonteir-o/intelligent-prompt-generator) | React, Gemini, rate limiting, Zod |
| [armando-blog](https://github.com/armandomonteir-o/armando-blog) | Next.js 16, headless WordPress |
| [nutri-joao](https://github.com/armandomonteir-o/nutri-joao) | Next.js App Router, SSG + CSR |

---

### How I work

- **Decisions in ADRs**, with the rejected alternatives and the trigger that would reopen each one.
- **Measure before and after.** A number I can't reproduce doesn't go in the README.
- **Tests in CI, deploys gated on them.** I'd rather break the build than break production.

**Stack:** TypeScript · Python · Node.js (NestJS, Fastify) · React · Next.js · PostgreSQL · Prisma · Google Cloud · Docker · GitHub Actions

<!-- card de estatísticas: entra quando o github-readme-stats próprio estiver no ar na Vercel (issue #1) -->

---

**Off the keyboard:** learning bass, listening to Brockhampton and RHCP. The Matrix is the reason I got into tech.

[LinkedIn](https://www.linkedin.com/in/armandoamonteiro/) · [Email](mailto:armandojr.ara@gmail.com)
