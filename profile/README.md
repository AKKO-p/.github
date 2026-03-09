<p align="center">
  <img src="https://raw.githubusercontent.com/AKKO-p/.github/main/profile/logo.svg" alt="AKKO" width="120" />
</p>

<h1 align="center">AKKO</h1>
<h3 align="center">Own Every Layer</h3>

<p align="center">
  Sovereign data platform — open-source alternative to Databricks, Snowflake, and Cloudera.<br/>
  From raw storage to AI-powered insights, every component runs on your infrastructure.
</p>

---

### What is AKKO?

AKKO (**A**nalytics **K**ernel, **K**eep **O**wnership) is a sovereign data platform that unifies 30+ open-source services into a turnkey lakehouse stack. It deploys via **Docker Compose** (development) or **Helm/Kubernetes** (production) behind a single reverse proxy with SSO.

| Layer | Components |
|-------|-----------|
| **Lakehouse** | MinIO (S3) + Apache Iceberg + Apache Polaris |
| **Compute** | Spark Connect, Trino (federated SQL) |
| **Notebooks** | JupyterHub (Python, R, Julia, VS Code, Quarto) |
| **BI & Orchestration** | Apache Superset, Apache Airflow 3 + OpenLineage |
| **Governance** | OpenMetadata (catalog, lineage, quality, glossary) |
| **Security** | Keycloak SSO (14 clients, 4 RBAC roles), OPA (row-level security, column masking) |
| **AI / LLM** | Ollama + LiteLLM gateway (Qwen 2.5, zero data leakage) |
| **Monitoring** | Prometheus, Grafana, Loki, AlertManager |

### Why AKKO?

- **Data sovereignty** -- every byte stays on your infrastructure (RGPD, DORA, NIS2, air-gapped)
- **No vendor lock-in** -- open standards (Iceberg, S3, SQL, OAuth2), swap any component
- **AI-native** -- local LLMs via Ollama + LiteLLM (OpenAI-compatible API), zero cloud costs
- **Fine-grained access** -- OPA policies for Trino: row-level security, column masking, ABAC
- **Two deployment modes** -- Docker Compose for dev, Helm/Kubernetes for production

### Quick Start

**Docker Compose:**

```bash
git clone https://github.com/AKKO-p/AKKO.git && cd AKKO
./scripts/start.sh
```

**Kubernetes (Helm):**

```bash
cd helm/scripts && bash deploy.sh
```

Open [https://localhost](https://localhost) (Docker) or [https://akko.local](https://akko.local) (k3d) to access the Cockpit portal.

### Repositories

| Repo | Description |
|------|-------------|
| [**AKKO**](https://github.com/AKKO-p/AKKO) | Platform source code, Helm charts, notebooks, documentation |
| [**akko-site**](https://github.com/AKKO-p/akko-site) | Landing page |
