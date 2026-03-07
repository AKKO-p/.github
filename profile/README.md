<p align="center">
  <img src="https://raw.githubusercontent.com/AKKO-p/.github/main/profile/logo.svg" alt="AKKO" width="120" />
</p>

<h1 align="center">AKKO</h1>
<h3 align="center">Own Every Layer</h3>

<p align="center">
  Sovereign data platform — zero licensing fees, zero vendor lock-in.<br/>
  From raw storage to polished dashboards, every component is open-source and runs on your infrastructure.
</p>

---

### What is AKKO?

AKKO (**A**nalytics **K**ernel, **K**eep **O**wnership) is a self-hosted data platform built on Docker Compose that replaces expensive cloud services like Databricks and Snowflake with 25+ integrated open-source components:

| Layer | Components |
|-------|-----------|
| **Lakehouse** | MinIO (S3) + Apache Iceberg + Apache Polaris |
| **Compute** | Spark Connect, Trino, DuckDB |
| **Notebooks** | JupyterHub (Python, R, Julia, code-server, Quarto) |
| **BI & Orchestration** | Apache Superset, Apache Airflow + OpenLineage |
| **Governance** | OpenMetadata (catalog, lineage, quality, glossary) |
| **Security** | Keycloak SSO (4 RBAC roles, 14 OAuth2 clients) |
| **Monitoring** | Prometheus, Grafana, Loki, Alertmanager |
| **AI** | Ollama + jupyter-ai (local LLM, zero data leaves) |

### Why AKKO?

- **Eliminate licensing costs** — 100% open-source, pay only for your own hardware
- **Data sovereignty** — every byte stays on your infrastructure (GDPR, HIPAA, NIS2)
- **No vendor lock-in** — open standards (Iceberg, S3, SQL, OAuth2), swap any component
- **One command** — `./scripts/start.sh` and you have a full data platform running

### Quick Start

```bash
git clone https://github.com/AKKO-p/AKKO.git
cd AKKO
./scripts/start.sh
```

Open [https://cockpit.localhost](https://cockpit.localhost) and you're in.
