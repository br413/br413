<div align="center">

# Senior Data Engineer & Data Architect

**Cloud data platforms · Lakehouse architecture · Production ETL pipelines · Data quality & observability**

[![GitHub followers](https://img.shields.io/github/followers/br413?style=flat-square&logo=github&label=Follow)](https://github.com/br413)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![dbt](https://img.shields.io/badge/dbt-transformations-FF694B?style=flat-square&logo=dbt&logoColor=white)](https://www.getdbt.com/)
[![Airflow](https://img.shields.io/badge/Apache-Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)](https://airflow.apache.org/)
[![Terraform](https://img.shields.io/badge/Terraform-IaC-844FBA?style=flat-square&logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Portfolio site](https://img.shields.io/badge/Website-br413.github.io-1f6feb?style=flat-square&logo=githubpages&logoColor=white)](https://br413.github.io/)
[![production-data-pipeline](https://img.shields.io/badge/Portfolio-production--data--pipeline-1f6feb?style=flat-square&logo=github)](https://github.com/br413/production-data-pipeline)
[![v0.1.0](https://img.shields.io/github/v/release/br413/production-data-pipeline?label=v0.1.0&style=flat-square)](https://github.com/br413/production-data-pipeline/releases/tag/v0.1.0)

</div>

---

## About

I design and build **cloud data platforms** that turn fragmented sources into reliable, observable, analytics-ready systems. My work spans **data engineering**, **data architecture**, and **platform automation** — incremental ETL pipelines, medallion lakehouse design, contract-driven data quality, and production operations on **AWS**, **Azure**, **Databricks**, and **Snowflake**.

```text
Design for failure.
Automate repeatable work.
Measure data quality.
Document decisions.
Keep systems understandable.
```

## Expertise

| Domain | Technologies & practices |
|--------|--------------------------|
| **Data engineering** | Python · SQL · incremental ingestion · ETL/ELT · API pipelines · checkpointing |
| **Data architecture** | Medallion lakehouse · bronze/silver/gold layers · lineage · governance · cost modeling |
| **Orchestration** | Apache Airflow · dbt · Prefect · Spark |
| **Cloud platforms** | AWS · Azure · Databricks · Snowflake |
| **Quality & observability** | Data contracts · schema validation · freshness checks · alerting · CI/CD |

## Data engineering portfolio

Production-style open-source projects with architecture docs, tests, CI, and operations runbooks.

| Project | What it demonstrates |
|---------|----------------------|
| [**production-data-pipeline**](https://github.com/br413/production-data-pipeline) | Incremental API ingestion · PostgreSQL bronze layer · dbt silver/gold models · Airflow orchestration · webhook alerts · [**v0.1.0 release**](https://github.com/br413/production-data-pipeline/releases/tag/v0.1.0) |
| [**data-quality-observability**](https://github.com/br413/data-quality-observability) | YAML data contracts · schema/null/uniqueness/freshness checks · check history · alert routing · Airflow scheduling |
| [**cloud-lakehouse-blueprint**](https://github.com/br413/cloud-lakehouse-blueprint) | Medallion architecture manifests · Terraform IaC · IAM governance · lineage graph · `validate --json` for CI |

## Open-source contributions

Contributions to widely used data-platform projects:

| Project | PR | Change |
|---------|-----|--------|
| [**Prefect**](https://github.com/PrefectHQ/prefect) | [#22500](https://github.com/PrefectHQ/prefect/pull/22500) ✓ merged | Document `/api/health` vs `/api/ready` for Kubernetes probes |
| [**Apache Airflow**](https://github.com/apache/airflow) | [#69857](https://github.com/apache/airflow/pull/69857) | Update SQLAlchemy pooling link to 2.0 docs |
| [**dbt docs**](https://github.com/dbt-labs/docs.getdbt.com) | [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606) | Troubleshooting note for prefixed custom schema names |

## Recent work

- **production-data-pipeline** — structured ingestion summary metrics, webhook alerts for zero-record runs and Airflow failures, local `scripts/check.ps1`
- **data-quality-observability** — customers data contract, `dqo_contract_checks` Airflow DAG (orders + customers)
- **cloud-lakehouse-blueprint** — `validate --json` for CI pipelines, deployment docs, changelog
- **Prefect** — merged upstream docs PR on Kubernetes health vs readiness probes

## Building in public

I publish focused, production-style data platform projects — not toy demos. Each repo includes architecture decision records, pytest coverage, GitHub Actions CI, and honest iteration through releases.

## Collaboration

Open to:

- Open-source **data platform** and **data engineering** contributions
- **Data architecture** reviews and lakehouse design discussions
- **Data quality**, **observability**, and **pipeline automation** tooling
- Technical collaboration with engineering teams and OSS maintainers

## GitHub activity

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=br413&show_icons=true&theme=default&hide_border=true&count_private=false)](https://github.com/br413)

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=br413&layout=compact&theme=default&hide_border=true)](https://github.com/br413)

</div>

---

**Website:** [br413.github.io](https://br413.github.io/) · **Portfolio:** [production-data-pipeline](https://github.com/br413/production-data-pipeline) · **Release:** [v0.1.0](https://github.com/br413/production-data-pipeline/releases/tag/v0.1.0) · **Lakehouse blueprint:** [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint) · **Data quality:** [data-quality-observability](https://github.com/br413/data-quality-observability)

**Focus areas:** data engineering · data architecture · cloud data platforms · lakehouse · ETL pipelines · dbt · Airflow · data quality · observability · Terraform · AWS · Azure · Databricks · Snowflake
