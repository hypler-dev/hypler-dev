# Hypler

**Independent software engineering · AI infrastructure · Data platforms**

[Website](https://hypler.com/) · [Engineering references](https://hypler.com/wiki) · [Contact](mailto:contact@hypler.com)

I build software at **Hypler**, an independent software company based in Las Vegas. My work spans native applications, agent infrastructure, backend services, data pipelines, and the interfaces that connect them. I work through the full system: architecture, implementation, persistence, integration, validation, and operational handoff.

Several substantial projects are being built in the open. The repositories show the implementation, design decisions, contracts, and development history behind the work.

## Building in the open

### [Rangoon](https://github.com/hypler-dev/rangoon)

A local-first desktop workbench for reusable AI capabilities. Rangoon organizes project instructions, skills, and workflows into versioned records that can be inspected, composed, compiled, and exported.

The implementation uses **Rust, Tauri 2, SQLite, and JavaScript/HTML/CSS**. Technical work includes immutable skill and workflow revisions, source provenance, deterministic instruction compilation, transactional persistence, backup and recovery, and explicit boundaries between the native host and renderer. Capability authoring works independently of external authorization providers.

### [LNSAT](https://github.com/hypler-dev/LNSAT)

An authorization and evidence engine for consequential agent actions. LNSAT separates what an agent can describe from permission to perform an exact operation and evidence of its outcome.

The source combines **Rust, TypeScript, and SQLite** around a Gateway boundary. Work covers versioned action contracts, deterministic policy, scoped approvals, one-time authorization consumption, bounded execution-attempt records, durable receipts, and reconciliation of uncertain results. MCP, API, CLI, and application interfaces share the same authority model.

### [VUSL](https://github.com/hypler-dev/vusl)

An independent semantic interoperability specification and experimental **Rust core**, supported by **Python conformance tooling**. VUSL describes native source identity, semantic fidelity, translation loss, relationships, evidence, and uncertainty explicitly.

Its engineering work includes canonical bytes, scoped identifiers, immutable typed results, bounded parsing, independent conformance expectations, and meaning-preservation checks. VUSL develops independently of Rangoon and LNSAT; Rangoon is its planned first consumer.

**Rangoon, LNSAT, and VUSL are in development.** Their repositories track implementation progress, validation, and release status. Planned integrations and platform targets are documented separately from delivered support.

## Commercial platform work

[**IZIOS**](https://hypler.com/projects/izios-diamond-platform) is a diamond data and commerce platform connecting supplier ingestion, normalized product records, structured and semantic search, customer workflows, and reusable APIs. Its June 2026 project record documents more than **1.8 million active and archived records** across the platform's catalog history.

The documented stack includes **React, TypeScript, Node.js, Express, PostgreSQL, and pgvector**. Work spans incremental synchronization, source-controlled availability, relational constraints, vector retrieval, administrative review, and boundaries between discovery, holds, and payments. The linked case study describes the platform; its full application is not an open-source release.

The public [**IZIOS Precious Metals Widgets**](https://github.com/hypler-dev/izios-precious-metals-widget) repository provides a smaller MIT-licensed component: embeddable JavaScript price displays and historical charts for gold, silver, platinum, and palladium.

## Technologies and where I use them

| Area | Technologies | Engineering focus |
| --- | --- | --- |
| Native systems | Rust, Tauri | Typed core logic, process boundaries, lifecycle and local applications |
| Applications and APIs | TypeScript, JavaScript, Node.js, Express | Interface contracts, backend services, integrations and reusable APIs |
| Web interfaces | React, HTML, CSS, Vite | Customer tools, administrative workflows and inspectable technical interfaces |
| Persistence and retrieval | PostgreSQL, SQLite, SQL, pgvector | Transactions, revision history, normalization, structured and vector search |
| Validation and tooling | Python, Rust tooling, GitHub Actions | Independent conformance tools, reproducible checks and CI |
| Agent interoperability | MCP, versioned JSON contracts, protocol adapters | Capability composition, scoped authority, provenance and evidence |

## Engineering priorities

- **Explicit contracts:** typed boundaries, validated inputs, versioned protocols, and defined failure states.
- **Durable state:** transactions, immutable revisions, dependency-aware changes, and recovery paths.
- **Accountable actions:** permissions, approvals, attempts, receipts, and unknown outcomes represented as distinct facts.
- **Source-aware data:** preserve origin, update context, availability, and the limits of a retrieved result.
- **Reviewable delivery:** documented decisions, conformance fixtures, CI, independent review, and release evidence.

For platform development, systems integration, or engineering collaboration: **[contact@hypler.com](mailto:contact@hypler.com)**.
