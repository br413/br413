<div align="center">

# Bobby Ray · Senior Data Engineer & Data Architect

**Data platforms where pipelines fail loudly — not silently**

[![GitHub followers](https://img.shields.io/github/followers/br413?style=flat-square&logo=github&label=Follow)](https://github.com/br413)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![dbt](https://img.shields.io/badge/dbt-transformations-FF694B?style=flat-square&logo=dbt&logoColor=white)](https://www.getdbt.com/)
[![Airflow](https://img.shields.io/badge/Apache-Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)](https://airflow.apache.org/)
[![Iceberg](https://img.shields.io/badge/Apache-Iceberg-0078D4?style=flat-square)](https://iceberg.apache.org/)
[![Terraform](https://img.shields.io/badge/Terraform-IaC-844FBA?style=flat-square&logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Portfolio site](https://img.shields.io/badge/Website-br413.github.io-1f6feb?style=flat-square&logo=githubpages&logoColor=white)](https://br413.github.io/)
[![lakehouse-platform-starter](https://img.shields.io/github/v/release/br413/lakehouse-platform-starter?label=lakehouse--platform&style=flat-square&color=238636)](https://github.com/br413/lakehouse-platform-starter/releases/tag/v1.0.0)
[![dbt docs](https://img.shields.io/badge/dbt%20docs-live-FF694B?style=flat-square&logo=dbt&logoColor=white)](https://br413.github.io/lakehouse-platform-starter/)

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

## Flagship project

<table>
<tr>
<td width="120"><strong>⭐ Lakehouse</strong></td>
<td>

**[lakehouse-platform-starter](https://github.com/br413/lakehouse-platform-starter)** — Runnable reference architecture: **Airflow + Cosmos** · **dbt** · **Iceberg** · **Trino** · **OpenLineage** · **Great Expectations**

[`make pipeline`](https://github.com/br413/lakehouse-platform-starter#quick-start) · [Live dbt docs](https://br413.github.io/lakehouse-platform-starter/) · [Interview walkthrough](https://github.com/br413/lakehouse-platform-starter/blob/main/docs/interview-walkthrough.md) · [**v1.0.0**](https://github.com/br413/lakehouse-platform-starter/releases/tag/v1.0.0)

</td>
</tr>
</table>

## Platform stack (portfolio)

Connected layers — not isolated demo repos:

| Layer | Project | Focus |
|-------|---------|-------|
| **Flagship · Lakehouse** | [**lakehouse-platform-starter**](https://github.com/br413/lakehouse-platform-starter) | Iceberg + Trino + Cosmos dbt + Airflow + Marquez + GE · Docker stack · CI · hosted docs |
| **Ingest & transform** | [**production-data-pipeline**](https://github.com/br413/production-data-pipeline) | Incremental API · PostgreSQL bronze · dbt · Airflow · [**v0.1.0**](https://github.com/br413/production-data-pipeline/releases/tag/v0.1.0) |
| **Quality & observability** | [**data-quality-observability**](https://github.com/br413/data-quality-observability) | YAML contracts · schema/freshness checks · run history · alerts |
| **Platform & governance** | [**cloud-lakehouse-blueprint**](https://github.com/br413/cloud-lakehouse-blueprint) | Medallion manifests · Terraform · IAM · lineage · CI validation |

## Expertise

| Domain | Technologies & practices |
|--------|--------------------------|
| **Data engineering** | Python · SQL · incremental ingestion · ETL/ELT · API pipelines · checkpointing · idempotent loads |
| **Data architecture** | Medallion lakehouse · Iceberg · bronze/silver/gold · lineage · governance · cost modeling |
| **Orchestration** | Apache Airflow · Cosmos · dbt · Prefect · Spark |
| **Cloud platforms** | AWS · Azure · Databricks · Snowflake |
| **Quality & observability** | Data contracts · Great Expectations · OpenLineage · schema validation · CI/CD |

## Open-source contributions

Production operations knowledge contributed upstream:

| Project | PR | Change |
|---------|-----|--------|
| [**Airflow**](https://github.com/apache/airflow) | [#70171](https://github.com/apache/airflow/pull/70171) | Surface dbt Cloud failure details in Airflow task logs |
| [**Prefect**](https://github.com/PrefectHQ/prefect) | [#22500](https://github.com/PrefectHQ/prefect/pull/22500) ✓ merged | Kubernetes readiness vs liveness probes |
| [**Prefect**](https://github.com/PrefectHQ/prefect) | [#22533](https://github.com/PrefectHQ/prefect/pull/22533) | Global concurrency limit setup docs (re-review requested) |
| [**dbt docs**](https://github.com/dbt-labs/docs.getdbt.com) | [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606) ✓ merged | Prefixed custom schema troubleshooting |

## Building in public

**Since 2026** — I publish production-style data platform work in the open: portfolio repos, upstream contributions, and technical writing. Prior employer work lived in private GitLab/Azure DevOps; this GitHub profile is my **public proof of craft**, not a full career timeline.

| What you'll find here | Where |
|----------------------|-------|
| Lakehouse + pipeline + quality + platform stack | Pinned repos |
| Upstream OSS (Prefect, dbt, Airflow) | [OSS table above](#open-source-contributions) |
| Architecture write-ups | [Dev.to](https://dev.to/bobby_ray_581732c715283b2) · [br413.github.io](https://br413.github.io/) |
| 90-day contribution plan | [docs/90-day-contribution-plan.md](docs/90-day-contribution-plan.md) |
| Daily activity log (automated) | [docs/contribution-log.md](docs/contribution-log.md) |

Each flagship repo includes ADRs, pytest coverage, GitHub Actions CI, operations runbooks, and documented trade-offs — not toy demos.

**Current focus (next 90 days):** land Airflow #70171 + Prefect #22533, open Airflow #43366 + Meltano #6289 PRs, release `production-data-pipeline` v0.2.0, publish article #2 on data quality contracts.

## Writing

| Article | Topic |
|---------|-------|
| [**Building a Production Data Pipeline with Incremental Loading and dbt**](https://dev.to/bobby_ray_581732c715283b2/building-a-production-data-pipeline-with-incremental-loading-and-dbt-2e2c) | Incremental checkpoints, idempotent loads, medallion layering, Airflow orchestration, failure modes |

More at [**br413.github.io**](https://br413.github.io/) · series: *Cloud Data Platform Patterns*

## Collaboration

Open to senior data engineering roles, data platform architecture discussions, and technical collaboration.

---

<div align="center">

**Website:** [br413.github.io](https://br413.github.io/) · **Flagship:** [lakehouse-platform-starter](https://github.com/br413/lakehouse-platform-starter) · **dbt docs:** [live](https://br413.github.io/lakehouse-platform-starter/)

`data engineering` · `lakehouse` · `dbt` · `Airflow` · `Iceberg` · `Trino` · `OpenLineage` · `Terraform`

</div>
