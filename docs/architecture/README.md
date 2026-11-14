# beautifulrust — Architecture Diagrams

Rendered with [Archify](https://github.com/tt-a1i/archify). Each entry is a standalone,
explorable HTML page (inline SVG, dark/light themes, live motion) paired with its source
JSON candidate. The set documents the backend-rust contract this repo's Rust guidance is
distilled from: an axum composition root over vertical feature slices, a warden security
crate, sqlx adapters behind ports, Postgres behind a pool, a zero-broker `email_jobs`
outbox drained by the loom worker, an OIDC provider and mail vendor as the only external
systems, and the boot → wire → serve → readyz runtime rail.

This repo ships no runtime service itself — it teaches the contract. Every component and
edge below comes from the backend-rust kit the Rust guidance is distilled from.

| Diagram | Type | What it shows | JSON | HTML |
|---|---|---|---|---|
| c4-containers | architecture | Container view: SDK clients → edge nginx → `<app>-api` (axum) with PostgreSQL 17 behind the sqlx pool, the OIDC provider in front of the warden guard, and mail + OTLP leaving through port traits — plus the build/run/quality-gate cards (cargo workspace, static Dockerfile, `just ci` = fmt + clippy pedantic + nextest) | [json](c4-containers.json) | [html](c4-containers.html) |
| services-slices | architecture | Package topology: the composition root, the feature slices (`auth`, `widgets`), the platform crates (`warden`, `ports`, `mailer`, `loom`) and the shared kernel, with the `email_jobs` state table as the outbox boundary — adapters live in `ports/src/adapters/*_pg.rs` behind repository traits | [json](services-slices.architecture.json) | [html](services-slices.architecture.html) |
| auth-algorithm | workflow | The auth algorithm as gated steps: signup → 6-digit code → outbox enqueue → verify → password-first login gates → JWT + rotating refresh with CAS replay defense, with the code-expiry, anti-enumeration and token rules on the cards | [json](auth-algorithm.workflow.json) | [html](auth-algorithm.workflow.html) |
| outbox-algorithm | workflow | Durable mail delivery on the zero-broker outbox: post-write enqueue on its own pool connection, claim CTE with `FOR UPDATE SKIP LOCKED` and a 5-minute lease, render + send, then backoff `2^n ±10%` to dead-letter — the dual-write window called out, not hidden | [json](outbox-algorithm.workflow.json) | [html](outbox-algorithm.workflow.html) |
| auth-sequence | sequence | The full auth request chain across client, API, Postgres, the outbox worker and the mail vendor: signup writes, enqueue, code delivery, verify, then login with the rotating refresh | [json](auth-sequence.sequence.json) | [html](auth-sequence.sequence.html) |
| outbox-sequence | sequence | The worker's message trace: enqueue after the write, at-least-once claim, render/send/ack → `mark_sent`, failure → retry `2^n` → dead-letter, and the hourly janitor purge | [json](outbox-sequence.sequence.json) | [html](outbox-sequence.sequence.html) |
| database-dataflow | dataflow | Where identity data goes: use-cases writing `users` / `sessions` / code tables and enqueuing `email_jobs` rows, the worker claiming them, and the sender shipping the message — with the ledgers and the janitor at the end | [json](database-dataflow.dataflow.json) | [html](database-dataflow.dataflow.html) |
| runtime-lifecycle | lifecycle | Process runtime states: typed-config boot → wire deps → http serve → readyz gate → request flow, with the drain loop, the 403 gate, the fail-closed config exit, the 503 degraded ending and the recovered worker path | [json](runtime-lifecycle.lifecycle.json) | [html](runtime-lifecycle.lifecycle.html) |

Authored with Archify, sibling set of the facta backend kits. The diagram content is
grounded in the backend-rust kit this repo's guidance comes from
(`ai-coding-playbook/rust`), with the crate names left as the `<app>` placeholder the
template ships.

Adapted for this repo, relative to the source set:

- `auth-algorithm` and `outbox-algorithm` were authored against workflow schema v1
  (fixed geometry) and are rendered as schema v2 (`readable-v2`). The v1 contract fixes
  the canvas at 720px wide, which the showcase viewport gate rejects; v2 measures the
  real footprint. The authored route and label pins were dropped so the v2 compiler
  routes the edges itself. Every node, edge, label and card is unchanged.
- `auth-sequence` and `database-dataflow` dropped their explicit `meta.viewBox`, so the
  renderer sizes the canvas and declares the reader fit. The authored geometry inside
  the canvas — participants, message positions, stages, nodes, flows and label pins — is
  unchanged.
