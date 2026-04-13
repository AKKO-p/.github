<p align="center">
  <img src="https://raw.githubusercontent.com/AKKO-p/.github/main/profile/logo.svg" alt="AKKO" width="120" />
</p>

<h1 align="center">AKKO</h1>
<h3 align="center">Own Every Layer</h3>

<p align="center">
  Sovereign analytics platform — open-source alternative to proprietary cloud solutions.<br/>
  From raw storage to AI-powered insights, every component runs on your infrastructure.
</p>

---

### What is AKKO?

AKKO (**A**nalytics **K**ernel, **K**eep **O**wnership) is a sovereign analytics platform that unifies 33+ open-source services into a turnkey lakehouse. It deploys via **Helm on Kubernetes** (k3d for dev, any k8s distribution for production) behind a single reverse proxy with SSO.

| Layer | Components |
|-------|-----------|
| **Lakehouse** | MinIO (S3) + Apache Iceberg + Apache Polaris |
| **Compute** | Spark Connect, Trino 480 (federated SQL) |
| **Notebooks** | JupyterHub (Python, R, Julia, VS Code, Quarto) |
| **BI & Orchestration** | Apache Superset, Apache Airflow 3 + OpenLineage |
| **Governance** | OpenMetadata 1.12.1 (catalog, lineage, quality, glossary) |
| **Semantic Layer** | dbt Core (versioned SQL transformations, metrics, data tests) |
| **Security** | Keycloak SSO (13 clients, 5 RBAC roles), OPA (row-level security, column masking), AI RBAC |
| **AI / LLM** | Ollama + LiteLLM gateway (Qwen 2.5, zero data leakage), 13 native Trino AI SQL UDFs |
| **AI Agents** | MCP Servers (Trino + OpenMetadata) for sovereign AI agents (Claude, Cursor) |
| **ML** | MLflow (experiment tracking, model registry, artifact store on MinIO) |
| **Monitoring** | Prometheus, Grafana, Loki, AlertManager |
| **Audit Trail** | 6 sources (Keycloak, OPA, Trino, Airflow, MinIO, OpenMetadata) aggregated in Loki, visualized in Grafana |

### Why AKKO?

- **Data sovereignty** -- every byte stays on your infrastructure (RGPD, DORA, NIS2, air-gapped)
- **No vendor lock-in** -- open standards (Iceberg, S3, SQL, OAuth2), swap any component
- **AI-native** -- local LLMs via Ollama + LiteLLM (OpenAI-compatible API), MCP servers for sovereign AI agents, 13 AI SQL functions in Trino, zero cloud costs
- **Fine-grained access** -- OPA policies for Trino: row-level security, column masking, ABAC. AI RBAC via OPA
- **Kubernetes-first** -- single `helm install` on k3d (dev), k3s, EKS, GKE, AKS, or bare-metal k8s. 29 sub-charts, 10 custom Docker images
- **Full audit trail** -- 6 event sources aggregated in Loki with Grafana dashboards for compliance (DORA, NIS2, RGPD)

### Quick Start

```bash
git clone https://github.com/AKKO-p/AKKO.git akko && cd akko && bash helm/scripts/deploy.sh
```

Open [https://akko.local](https://akko.local) to access the Cockpit portal.

### Repositories

| Repo | Description |
|------|-------------|
| [**AKKO**](https://github.com/AKKO-p/AKKO) | Platform source code, Helm charts, notebooks, documentation |
| [**akko-site**](https://github.com/AKKO-p/akko-site) | Landing page |
