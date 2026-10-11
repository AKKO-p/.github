<p align="center">
  <img src="https://raw.githubusercontent.com/AKKO-p/.github/main/profile/logo.svg" alt="AKKO" width="96" />
</p>

<h1 align="center">AKKO</h1>
<h3 align="center">Governed access for AI agents to the data you already have</h3>

<p align="center">
  AKKO is a French project building a sovereign data and AI platform that runs on your own
  infrastructure, under your own rules. Its first open building block lets AI agents read
  enterprise data with the rights of the person they work for, and nothing more.
</p>

<p align="center">
  <a href="https://akko-ai.com">akko-ai.com</a> ·
  <a href="https://akko-ai.com/en/docs/akko-mcp-trino/">Documentation</a> ·
  <a href="mailto:contact@akko-ai.com">contact@akko-ai.com</a>
</p>

---

## akko-mcp-trino, the open source core

[**AKKO-p/akko-mcp-trino**](https://github.com/AKKO-p/akko-mcp-trino) is an MCP server for
Trino, under the Apache 2.0 licence.

- **Six read-only tools.** List catalogs, schemas and tables, describe a table, explain a
  query and run it. Every statement is parsed, and a write anywhere in it is refused before
  Trino.
- **The user's own rights, end to end.** In `jwt` mode, the user's verified token goes to
  Trino, which verifies it again and runs the query as that person: Ranger or OPA decide for
  each user, not for a service account. Two users asking the same question get the answers
  their own rights allow.
- **Bounded and audited.** Row and time limits on every call, one audit line per call, and
  no token ever written to the logs.

```bash
pip install akko-mcp-trino        # or: uvx akko-mcp-trino
```

It works with any MCP host (Claude, Cursor, VS Code, Mistral Vibe, the Python SDK) and any
model, since the server never talks to a model.

## The AKKO platform

Beyond this core, AKKO assembles the layers of a data and AI platform (query engine, catalog,
storage, notebooks, governance, observability, AI assistants), each replaceable, installed on
Kubernetes in your own environment. Read more on [akko-ai.com](https://akko-ai.com).

## Contributing

Issues and pull requests are welcome on
[akko-mcp-trino](https://github.com/AKKO-p/akko-mcp-trino/issues). Security reports go to
[security@akko-ai.com](mailto:security@akko-ai.com), as described in its
[SECURITY.md](https://github.com/AKKO-p/akko-mcp-trino/blob/main/SECURITY.md).

---

<p align="center"><sub>AKKO · Analytics Kernel, Keep Ownership · 🇫🇷 Un projet français</sub></p>
