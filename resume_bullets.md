# PointAura: resume bullets and project note

## Resume bullets

- **Designed and built PointAura solo, an AI natural-language BI platform on xAI Grok** (~29K lines of core Python, 145 commits, Apr 2025 to Sep 2026). Users describe a chart in plain English. A two-stage LangChain pipeline generates dialect-correct SQL against live PostgreSQL, MySQL, SQL Server, Azure SQL, or Snowflake sources, then generates Plotly code that runs under a timeout and renders in multi-pane Dash dashboards.
- **Refactored a single-file Dash prototype into a layered platform.** Built a typed domain layer, a JWT-secured Flask REST API (~35 endpoints, credential redaction, ownership-by-404), and a thin UX with concurrent per-pane render workers. Then added hub-and-spoke multi-org hosting with role-based access, plus affiliate SSO using HMAC-signed, short-lived tokens.
- **Shipped an MCP server (JSON-RPC 2.0) with 8 tools** that lets external AI agents register data sources and have Grok propose and apply whole dashboard pages. Cut LLM spend with "TokenSaver," which caches approved SQL and chart code so later loads skip model calls entirely.

## Project note (for application forms, e.g. "a project you're proud of")

I designed and built PointAura on my own, using AI coding assistants. It's a natural-language BI platform where you type "monthly revenue by region as a stacked area chart" and xAI Grok writes the SQL for your live database and the Plotly code to chart it. I took it from a single-file prototype to a layered platform with a JWT REST API, five database connectors, multi-org hosting, SSO, an MCP server that lets AI agents build dashboards, and a caching layer that removes repeat LLM cost.
