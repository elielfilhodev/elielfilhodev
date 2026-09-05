# Eliel Filho

**Full Stack Developer** — TypeScript, Java, Node.js, Next.js  
São Paulo, Brazil · Remote or hybrid · Open to opportunities

[LinkedIn](https://linkedin.com/in/eliel-filho-dev/) · [Portfolio](https://elieldev-web.vercel.app) · [Email](mailto:elielfilholk@gmail.com)

---

## About

I build software at the point where engineering meets real retail operations. I run the e-commerce of a mobile phone retail chain, which means I don't ship a feature and move on — I stay with the broken checkout, the stock mismatch and the support ticket at 9pm.

That shaped how I work. I favor predictable, maintainable architecture over clever abstraction, and I design for the failure case first: the offline machine, the payment gateway timeout, the tax rule that changes next quarter.

---

## Stack

| Area | Tools |
|:--|:--|
| **Languages** | TypeScript, JavaScript, Java, Python, Go, SQL |
| **Frontend** | Next.js, React, Vue, Tailwind, shadcn/ui |
| **Backend** | NestJS, Fastify, Express, Spring Boot |
| **Data** | PostgreSQL, SQL Server, SQLite, Redis |
| **Infrastructure** | Docker, Kubernetes, Terraform, GitHub Actions, Linux, AWS |

---

## Selected work

### meucarinho.com.br — AI music platform

*Solo product, from landing page to payment and delivery.*  
`Next.js` · `TypeScript` · `Node.js` · `PostgreSQL` · `Redis` · `Docker`

Generation runs asynchronously with state persisted at every step: the customer pays, gets immediate confirmation, and heavy processing happens outside the request cycle. The payment webhook is idempotent, because gateways resend notifications and double-charging is an incident, not a bug.

[meucarinho.com.br →](https://meucarinho.com.br)

### luthierhossony.com — Institutional site

*Storefront and lead capture for a professional luthier.*  
`HTML` · `CSS` · `JavaScript`

Built without a framework on purpose. The problem was a storefront, not an application; a framework would have added bundle size, a build step and maintenance surface with nothing in return. Choosing the smaller tool is an engineering decision, not the absence of one.

[luthierhossony.com →](https://luthierhossony.com)

### E-commerce operations and internal tooling

*Catalog, stock, checkout, marketplaces and support for a retail chain, plus the automation behind it.*  
`Python` · `TypeScript` · `SQL Server` · `PostgreSQL`

Every automation that touches sales data ships with structured logging, idempotent execution and a dry-run mode before it writes to production. A script running unattended against an ERP has to be auditable afterwards, and it has to fail safely rather than halfway.

---

## How I build

- **Layered and decoupled.** Route → service → repository, with external integrations behind an interface. Replacing a payment gateway should be a new implementation, not a domain refactor.
- **Validation at the edge.** Nothing unvalidated crosses the application boundary. Errors are handled explicitly, never swallowed.
- **Relational by default.** Business data has shape, and referential integrity is the last line of defense when the application gets it wrong. Redis is cache and queue — never the source of truth.
- **Security as routine, not audit.** Parameterized queries, explicit output DTOs, Argon2/bcrypt hashing with short-lived tokens, authorization enforced in the service layer, secrets in a vault, dependency scanning in CI.
- **Reproducible deployment.** Multi-stage Docker builds running as a non-root user, health checks and resource limits, lint and tests blocking merge. Deploys should be boring and repeatable.
- **Tests where the risk is.** Business rules, calculations, external integrations and error paths. High coverage on trivial code is a pretty, useless metric.

---

## Education

**Full Stack Java** — EBAC, 2026  
**Technical Degree in Systems Analysis and Development** — ETEC de Taquarituba, 2021

---

## Contact

If you're hiring for full stack, frontend or backend roles in e-commerce, payment products or internal tooling, I'd be glad to talk.

[LinkedIn](https://linkedin.com/in/eliel-filho-dev/) · [Portfolio](https://elieldev-web.vercel.app) · [elielfilholk@gmail.com](mailto:elielfilholk@gmail.com)
