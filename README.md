# Arkar Than Htike | Backend Engineer

**API Infrastructure · Database Migrations · Event-Driven Architecture**

[Technical Focus](#technical-focus) · [Tech Stack](#tech-stack) · [Current Focus](#current-focus)

I focus on backend infrastructure, database compatibility, and automation for reliable transaction-data integrations.

My engineering interests center on explicit API contracts, predictable failure handling, and preserving data integrity as systems evolve.

## Technical Focus

- **API Infrastructure:** API gateways, gRPC interfaces, timeout budgets, and controlled retries.
- **Database Migrations:** Schema evolution, compatibility checks, transaction boundaries, and recovery strategies.
- **Event-Driven Architecture:** Idempotency, duplicate handling, replay semantics, and backpressure.
- **Backend Automation:** Reproducible diagnostics, targeted patch generation, and isolated regression testing.

## Tech Stack

| Category | Technologies |
| :--- | :--- |
| Languages | Python · Go · TypeScript |
| Runtime | Node.js |
| Databases | PostgreSQL · MySQL |
| Data Access | SQLAlchemy · Prisma |
| Tools / Gateways | Kong · gRPC |
| DevOps | Docker |

## Current Focus

### CLEAR — Change Remediation for Transaction-Data Connectors

I am building **CLEAR**, a change-remediation tool for bank integration engineers.

The initial problem is specific: **an upstream database schema change breaks a transaction-data connector after an update.**

CLEAR's intended workflow:

1. **Detect** schema changes against a versioned baseline.
2. **Diagnose** incompatibilities in connector queries and field mappings.
3. **Generate** narrow candidate patches for supported change patterns.
4. **Verify** patches in an isolated environment using synthetic transactions.
5. **Present** the code changes and test evidence for engineering approval.

**Primary verification objective:** Restore connector compatibility while checking that expected test transactions are neither missing nor duplicated.

**Status:** Prototype development. Automated remediation and verification are development objectives, not claims of production deployment.

## Engineering Principles

- **Correctness first:** Verify transaction identifiers and values, not only row counts.
- **Explicit failure handling:** Bound retries and make partial failures observable.
- **Reproducibility:** Tie proposed fixes to source revisions, schema baselines, and test fixtures.
- **Minimal changes:** Keep generated patches narrow and reviewable.
- **Human approval:** Require engineering review before changes enter deployment workflows.

## Collaboration

Interested in backend projects involving API gateways, database migrations, integration reliability, and developer tooling.

[Find me on GitHub → @Htike-tech](https://github.com/Htike-tech)
