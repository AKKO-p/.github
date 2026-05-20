<p align="center">
  <img src="https://raw.githubusercontent.com/AKKO-p/.github/main/profile/logo.svg" alt="AKKO" width="120" />
</p>

<h1 align="center">AKKO</h1>
<h3 align="center">AI Runtime for regulated European workloads</h3>

<p align="center">
  Orchestrate, govern, audit and optimise private LLMs on your infrastructure.<br/>
  Six proprietary components on top of an open-source Lego foundation.<br/>
  Built for <strong>banking</strong>, <strong>healthcare</strong> and the <strong>public sector</strong>.
</p>

<p align="center">
  <a href="https://akko-ai.com/runtime">akko-ai.com/runtime</a> &middot;
  <a href="https://akko-ai.com">akko-ai.com</a> &middot;
  <a href="mailto:hello@akko-ai.com">hello@akko-ai.com</a>
</p>

---

## The AKKO model: Open Blueprints + Open Lab + Closed Runtime

AKKO is not a single-license product. The foundation is open, the lab is open,
the runtime is commercial. This is the honest model that lets regulated buyers
audit what they install, while the proprietary engine keeps your prompts and
governance under a signed contract.

| 📦 Open Blueprints | 🧪 Open Lab | 🔒 Closed Runtime |
|---|---|---|
| **Apache 2.0** | **Apache 2.0** | **Commercial license** |
| Helm charts, Terraform modules, agent templates, integration glue. | 30+ notebooks across banking, healthcare and retail. Lab kernels, Spark Connect examples, dbt marts, sample governed pipelines. | 17 SQL AI functions, NL2SQL orchestrator, governance engine, observability layer, catalog manager, control plane. |
| Free to fork and audit. | Free to fork and contribute. | Signed EULA via Harbor private registry. |
| Public on GitHub. | Public on GitHub. Drives the [try.akko-ai.com](https://akko-ai.com/runtime) sandbox. | [Request access](mailto:hello@akko-ai.com) for the proprietary core. |

> **We are honest about this:** AKKO is not 100 % open source. The blueprints
> and the lab are. The runtime is the product, distributed under a commercial
> license to organisations that need a signed contract for their AI
> infrastructure.

---

## Public repositories

The five Apache 2.0 repositories below carry the **Open Blueprints** and
**Open Lab** layers of the model. They land progressively during Sprint 86.
A "⭐ coming soon" tag means the repo is scaffolded but not yet public.

| Repo | Layer | What it ships | Status |
|---|---|---|---|
| [`AKKO-p/sovereign-blueprints`](https://github.com/AKKO-p/sovereign-blueprints) | 📦 Blueprints | Helm overlays for banking, healthcare and public sector. Glue scripts. Reference values files. | ⭐ coming soon (Sprint 86-H1) |
| [`AKKO-p/akko-runtime-sdk`](https://github.com/AKKO-p/akko-runtime-sdk) | 📦 Blueprints | Python SDK to call the Runtime: ADEN, RAG, Catalog, Governance. Open client, closed engine. | ⭐ coming soon (Sprint 86-H2) |
| [`AKKO-p/akko-lab-blueprints`](https://github.com/AKKO-p/akko-lab-blueprints) | 🧪 Lab | 30+ Jupyter notebooks across verticals. Lab kernels. Spark Connect + federated SQL examples. | ⭐ coming soon (Sprint 86-H3) |
| [`AKKO-p/akko-mtls-blueprints`](https://github.com/AKKO-p/akko-mtls-blueprints) | 📦 Blueprints | Service-mesh mTLS wrapper. Kyverno + cosign policy bundles. | ⭐ coming soon (Sprint 86-H4) |
| [`AKKO-p/akko-ocsf-schemas`](https://github.com/AKKO-p/akko-ocsf-schemas) | 📦 Blueprints | OCSF-aligned audit + lineage + ADEN + RAG event schemas. Validators. | ⭐ coming soon (Sprint 86-H5) |

> The **proprietary runtime** lives in private repositories on AKKO's GitHub
> organisation. Access is granted to customers under a signed EULA via a
> private Harbor registry. [Talk to us](mailto:hello@akko-ai.com).

---

## What is the AKKO AI Runtime?

The Runtime is the layer that turns a Kubernetes cluster into a sovereign AI
platform. Six proprietary components, layered on top of an open-source stack
the customer already controls:

| Component | Layer | Purpose |
|---|---|---|
| **ADEN** | AI | Natural language to governed SQL, with audit receipts. |
| **RAG** | AI | Sovereign knowledge bases over your private corpus. |
| **Catalog Manager** | Catalog | Self-service onboarding for any source (Postgres, Oracle, Hive, Snowflake, Databricks, MongoDB, Kafka…). |
| **Governance Engine** | Governance | Row-level filtering, column masking, RBAC propagated across every layer. |
| **Observability Layer** | Observability | Unified metrics, logs, traces and AI Ops dashboards. |
| **Control Plane** | Cockpit | Single pane of glass for operators, analysts and stewards. |

The runtime is positioned on top of the AKKO Lego foundation — Compute,
Query, Catalog, Storage, BI, Lab, AI, Governance, Observability — so every
layer can be swapped, audited or extended without touching the runtime
contract.

[**See the full Runtime page →**](https://akko-ai.com/runtime)

---

## Try the sandbox

A live, read-only sandbox of the AKKO stack is coming online in **Q2 2026**:

- **URL** — [`try.akko-ai.com`](https://akko-ai.com/runtime) (coming soon)
- **Auto-login**, no credit card
- Banking, healthcare and retail seed datasets
- Drive the cockpit, ADEN, RAG, Lab and BI layers directly

The sandbox is read-only: it lets prospects feel the runtime without exposing
the proprietary code or our customers' data.

---

## Talk to us

| Channel | Audience |
|---|---|
| [hello@akko-ai.com](mailto:hello@akko-ai.com) | Pilots, regulated procurement, partnership |
| [akko-ai.com](https://akko-ai.com) | Product overview, layers, live screens |
| [akko-ai.com/runtime](https://akko-ai.com/runtime) | The Runtime page — six components + architecture diagram |
| LinkedIn `Building AKKO` | Public-facing engineering posts |
| X [`@akkoplatform`](https://x.com/akkoplatform) | Product announcements |

---

<p align="center"><sub>AKKO &middot; Analytics Kernel, Keep Ownership</sub></p>
