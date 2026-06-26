## Burnside Project - Building the Operational Context Ecosystem for AI Agents

<p align="center">
  <img src="home.png" alt="Burnside Project">
</p>

Most organizations have already invested heavily in operational systems, databases, SaaS platforms, APIs, and analytics infrastructure. As AI agents become part of daily workflows, a new challenge emerges:

#### How do AI agents safely access trusted business context without direct access to production systems?

Today’s AI ecosystem has no equivalent of a website, email address, or phone number for operational business context. Every organization is rebuilding custom integrations, permissions, and data access patterns for every new AI application.

We believe AI agents need governed operational context—not database credentials.

Burnside Project is building an open ecosystem that helps organizations:

* Capture operational reality from production systems
* Govern access through policy, identity, and data classification
* Model business entities, relationships, and operational context
* Publish trusted context through secure AI endpoints
* Enable AI agents to safely access business information

## What AI Applications and Agents Can You Build?

### Customer Support Agents

Customer: "Where is my order?"

Instead of searching multiple systems, an AI agent can access governed order history, shipment status, inventory, and support interactions.

Powered by:
- pg-cdc
- Business Context Models
- ai-dial-pad

---

### Customer Success Copilots

"What customers are at risk of churn?"

An AI agent can combine subscription activity, support tickets, usage trends, and account history to help customer success teams prioritize outreach.

Powered by:
- pg-cdc
- first-table
- ai-dial-pad

---

### Sales Assistants

"Which opportunities are most likely to close this quarter?"

AI agents can reason over operational data, customer activity, product adoption, and account history without direct production database access.

Powered by:
- pg-cdc
- first-table
- ai-dial-pad

---

### Operations Copilots

"What changed yesterday?"

AI agents can monitor operational activity, inventory movement, order delays, and fulfillment bottlenecks across the business.

Powered by:
- pg-cdc
- ai-dial-pad

---

### Executive Intelligence Agents

"Give me a morning briefing."

AI agents summarize business performance using governed operational context rather than manually assembled reports.

Powered by:
- Business Context Models
- Operational Context Publishing

---

## Our Projects - For turning operational data into AI-ready business context

### pg-cdc

A single-binary PostgreSQL change-data-capture daemon that streams WAL into typed Parquet files on cloud storage. Pure Go, no CGO, no Kafka, no JVM. Produces an immutable, governed data zone that downstream consumers (Athena, Spark, Iceberg-aware engines, AI agents via the MCP server) read from without ever touching the source database

https://github.com/burnside-project/pg-cdc

---
### ai-dial-pad(in Private Beta)

Publish governed data products as **dial-able tiny-URL MCP endpoints** — paste the URL into Claude or ChatGPT Enterprise and start a governed, audited conversation with your data.

https://github.com/burnside-project/burnside-project-ai-dial-pad

---

### pg-warehouse

The data platform is built from 5 independent projects across 4 layers. Each layer has a clear responsibility and communicates via Iceberg tables in a shared Glue catalog.

https://github.com/burnside-project/pg-warehouse

---
### wire-drop (in private beta)

Secure data exchange subscriber. Publishers push data over mTLS; wire-drop receives, deduplicates, writes Iceberg tables, and enforces tag-based governance.

---

### pg-collector
pg-collector is a lightweight edge compute agent that extracts PostgreSQL telemetry, processes it locally through a DuckDB analytical warehouse, and delivers Parquet files to our cloud platform where AI analyzes patterns and predicts issues before they impact your users.

Single binary. Zero runtime dependencies. YAML config. Runs anywhere — systemd, Docker, Kubernetes, bare metal.

https://github.com/burnside-project/pg-collector

---

## Architecture

Production Systems
→ Capture
→ Govern
→ Model
→ Publish
→ AI Agents

No direct AI access to production databases.

Just trusted business context.

Build Locally. Scale Intentionally.

---
### Why We Exist

> Modern analytics stacks have become expensive, complex, and difficult to govern.

Organizations spend hundreds of thousands of dollars per year on data warehouses, ETL pipelines, governance tools, and AI integrations.

--- 
### Burnside Project provides a simpler alternative:

* Open formats
* Local-first analytics
* Bring-your-own-cloud
* PostgreSQL-native
* AI-ready governance
* No vendor lock-in

---

### Principles

* Security by design
* Governance first
* Open standards
* Local development experience
* Multi Cloud
* AI enablement without production access

---

### Community

* Website: https://burnsideproject.ai
* GitHub: https://github.com/burnside-project
* Substack: https://burnsideproject.substack.com
* LinkedIn: https://www.linkedin.com/company/burnside-project

---

### Current Focus

Building the open infrastructure stack for governed AI and PostgreSQL intelligence.
