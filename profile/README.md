## Burnside Project

<p align="center">
  <img src="home.png" alt="Burnside Project">
</p>


Open infrastructure for governed analytics, PostgreSQL intelligence, and AI-ready data products.

We believe organizations should own their data, govern AI access, and build analytics without warehouse lock-in.

## Projects

---

### pg-cdc

The security boundary between production PostgreSQL databases and AI agents.

Streams WAL changes into typed, compacted Parquet files in cloud storage. Creates a physical air gap — agents and developers query governed, immutable data without ever touching production. Pure Go. No CGO. Single binary.

https://github.com/burnside-project/pg-cdc

---
### pg-warehouse

The data platform is built from 5 independent projects across 4 layers. Each layer has a clear responsibility and communicates via Iceberg tables in a shared Glue catalog.

https://github.com/burnside-project/pg-warehouse

---
### wire-drop (in private beta)

Secure data exchange subscriber. Publishers push data over mTLS; wire-drop receives, deduplicates, writes Iceberg tables, and enforces tag-based governance.

---
### ai-dial-pad(in Private Beta)

Publish governed data products as **dial-able tiny-URL MCP endpoints** — paste the URL into Claude or ChatGPT Enterprise and start a governed, audited conversation with your data.

---
### pg-collector
pg-collector is a lightweight edge compute agent that extracts PostgreSQL telemetry, processes it locally through a DuckDB analytical warehouse, and delivers Parquet files to our cloud platform where AI analyzes patterns and predicts issues before they impact your users.

Single binary. Zero runtime dependencies. YAML config. Runs anywhere — systemd, Docker, Kubernetes, bare metal.

https://github.com/burnside-project/pg-collector

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

Security by design
Governance first
Open standards
Local development experience
Cloud optional
AI enablement without production access

---

### Community

* Website: https://burnsideproject.ai
* GitHub: https://github.com/burnside-project
* Substack: https://burnsideproject.substack.com
* LinkedIn: https://www.linkedin.com/company/burnside-project

---

### Current Focus

Building the open infrastructure stack for governed AI and PostgreSQL intelligence.
