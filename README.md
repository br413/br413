<div align="center">

# Bobby Ray · Senior Data Engineer & Data Architect

**Data platforms where pipelines fail loudly — not silently**

[![GitHub followers](https://img.shields.io/github/followers/br413?style=flat-square&logo=github&label=Follow)](https://github.com/br413)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![dbt](https://img.shields.io/badge/dbt-transformations-FF694B?style=flat-square&logo=dbt&logoColor=white)](https://www.getdbt.com/)
[![Airflow](https://img.shields.io/badge/Apache-Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)](https://airflow.apache.org/)
[![Terraform](https://img.shields.io/badge/Terraform-IaC-844FBA?style=flat-square&logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Portfolio site](https://img.shields.io/badge/Website-br413.github.io-1f6feb?style=flat-square&logo=githubpages&logoColor=white)](https://br413.github.io/)
[![Dev.to](https://img.shields.io/badge/Dev.to-technical%20writing-0a0a0a?style=flat-square&logo=devdotto&logoColor=white)](https://dev.to/bobby_ray_581732c715283b2)
[![production-data-pipeline](https://img.shields.io/github/v/release/br413/production-data-pipeline?label=production--data--pipeline&style=flat-square)](https://github.com/br413/production-data-pipeline/releases/tag/v0.1.0)

</div>

---

## About

I design and build **cloud data platforms** that survive partial failures, schema drift, and operational scale — incremental ingestion with checkpoint recovery, contract-driven data quality, medallion lakehouse patterns, and CI-validated platform automation on **AWS**, **Azure**, **Databricks**, and **Snowflake**.

Senior data engineering, to me, is **judgment under constraint**: intentional trade-offs, failure-aware design, and systems the next team can actually operate.

```text
Design for failure.
Automate repeatable work.
Measure data quality.
Document decisions.
Keep systems understandable.
```

## What senior looks like in my work

| Signal | How it shows up |
|--------|-----------------|
| **System design** | Architecture docs, ADRs, and clear boundaries between ingestion, transform, quality, and platform layers |
| **Failure handling** | Checkpoint recovery, idempotent loads, quality gates before bronze, operations runbooks |
| **Operational proof** | pytest, GitHub Actions CI, smoke tests, alert routing, and honest trade-off documentation |

## Platform stack (portfolio)

Three connected layers — not isolated demo repos:

| Layer | Project | Focus |
|-------|---------|-------|
| **1 · Ingest & transform** | [**production-data-pipeline**](https://github.com/br413/production-data-pipeline) | Incremental API ingestion · PostgreSQL bronze · dbt silver/gold · Airflow · webhook alerts · [**v0.1.0**](https://github.com/br413/production-data-pipeline/releases/tag/v0.1.0) |
| **2 · Quality & observability** | [**data-quality-observability**](https://github.com/br413/data-quality-observability) | YAML data contracts · schema/null/uniqueness/freshness checks · run history · alert routing |
| **3 · Platform & governance** | [**cloud-lakehouse-blueprint**](https://github.com/br413/cloud-lakehouse-blueprint) | Medallion manifests · Terraform IaC · IAM governance · lineage · `validate --json` for CI |

**Outcome:** pipelines that fail loudly, contracts that catch drift early, and platform patterns teams can run without tribal knowledge.

## Expertise

| Domain | Technologies & practices |
|--------|--------------------------|
| **Data engineering** | Python · SQL · incremental ingestion · ETL/ELT · API pipelines · checkpointing · idempotent loads |
| **Data architecture** | Medallion lakehouse · bronze/silver/gold layers · lineage · governance · cost modeling |
| **Orchestration** | Apache Airflow · dbt · Prefect · Spark |
| **Cloud platforms** | AWS · Azure · Databricks · Snowflake |
| **Quality & observability** | Data contracts · schema validation · freshness checks · alerting · CI/CD |

## Writing

| Article | Topic |
|---------|-------|
| [**Building a Production Data Pipeline with Incremental Loading and dbt**](https://dev.to/bobby_ray_581732c715283b2/building-a-production-data-pipeline-with-incremental-loading-and-dbt-57md) | Incremental checkpoints, idempotent loads, medallion layering, Airflow orchestration, failure modes, and scale trade-offs |

More at [**br413.github.io**](https://br413.github.io/) · series: *Cloud Data Platform Patterns*

## Open-source contributions

Production operations knowledge contributed upstream:

| Project | PR | Change |
|---------|-----|--------|
| [**Prefect**](https://github.com/PrefectHQ/prefect) | [#22500](https://github.com/PrefectHQ/prefect/pull/22500) ✓ merged | Kubernetes readiness vs liveness probes for orchestrator deployments |
| [**Prefect**](https://github.com/PrefectHQ/prefect) | [#22533](https://github.com/PrefectHQ/prefect/pull/22533) | Clarify global concurrency limit setup for production deployments |
| [**dbt docs**](https://github.com/dbt-labs/docs.getdbt.com) | [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606) | Troubleshooting note for prefixed custom schema names |

## Building in public

I publish focused, production-style data platform projects — not toy demos. Each flagship repo includes architecture decision records, pytest coverage, GitHub Actions CI, operations runbooks, and documented trade-offs.

## Collaboration

Open to:

- **Senior data engineering** and **data platform architect** roles
- **Data architecture** reviews and lakehouse design discussions
- **Data quality**, **observability**, and **pipeline automation** tooling
- Technical collaboration with engineering teams and OSS maintainers

---

**Website:** [br413.github.io](https://br413.github.io/) · **Writing:** [Dev.to](https://dev.to/bobby_ray_581732c715283b2) · **Flagship:** [production-data-pipeline](https://github.com/br413/production-data-pipeline) · **Quality:** [data-quality-observability](https://github.com/br413/data-quality-observability) · **Platform:** [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint)

**Focus areas:** data engineering · data architecture · cloud data platforms · lakehouse · ETL pipelines · dbt · Airflow · data contracts · observability · Terraform · AWS · Azure · Databricks · Snowflake
