# br413 · Senior Data Engineer & Data Architect

I build data pipelines and lakehouse platforms with **Python, SQL, Airflow, dbt, and Terraform**, focusing on recovery, data quality, and maintainability.

My work addresses interrupted ingestion, duplicate records, schema drift, and difficult operational handoffs through checkpoint recovery, idempotent loads, data contracts, and documented design decisions.

**Senior data engineering roles · Long-term data platform maintenance**

[Email: br198064@gmail.com](mailto:br198064@gmail.com) · [Portfolio](https://br413.github.io/) · [Selected Airflow implementation](https://github.com/apache/airflow/pull/70171)

## Selected evidence

- **Reviewed upstream implementation:** [Airflow #70171](https://github.com/apache/airflow/pull/70171), merged **September 14, 2026**. Added dbt Cloud failure details to task logs across the hook, operator, and sensor, with unit tests and maintainer review.
- **Runnable lakehouse reference:** [lakehouse-platform-starter](https://github.com/br413/lakehouse-platform-starter) — Airflow + Cosmos, dbt, Iceberg, Trino, OpenLineage, and Great Expectations. [Quick start](https://github.com/br413/lakehouse-platform-starter/blob/main/docs/QUICKSTART.md) · [Design decisions](https://github.com/br413/lakehouse-platform-starter/tree/main/docs/decisions) · [Backfill runbook](https://github.com/br413/lakehouse-platform-starter/blob/main/docs/runbooks/backfill-safety.md).

## Portfolio: problems, implementation, and review paths

These are public reference implementations and demonstrations. They show engineering decisions and reproducible behavior; they do not establish client deployments, production scale, or customer outcomes. Prior employer work lived in private GitLab/Azure DevOps; this portfolio is not a full employment history.

| Project | Problem addressed | Evidence to review |
| --- | --- | --- |
| [lakehouse-platform-starter](https://github.com/br413/lakehouse-platform-starter) | Reproducible lakehouse setup and safe backfills | DuckDB and Trino/Iceberg paths, dbt tests, lineage, [walkthrough](https://github.com/br413/lakehouse-platform-starter/blob/main/docs/interview-walkthrough.md) |
| [production-data-pipeline](https://github.com/br413/production-data-pipeline) | Interrupted ingestion, duplicate delivery, bad records | Checkpoints, PostgreSQL landing, quarantine, dbt, [operations runbook](https://github.com/br413/production-data-pipeline/blob/main/docs/operations.md); production Airflow deployment is outside the demo scope |
| [data-quality-observability](https://github.com/br413/data-quality-observability) | Invalid CSV deliveries and hard-to-inspect quality failures | YAML contracts, deterministic broken-to-fixed demo, offline HTML/JSON reports, SQLite history |
| [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint) | Reviewing storage, access, and governance before deployment | Manifests, S3/IAM/Glue Terraform modules, lineage, CI validation; live AWS deployment is outside the demo scope |

## Data platform maintenance

For teams seeking ongoing platform ownership, the maintenance work I can discuss includes:

- **Pipeline reliability:** investigate failed runs, repair ingestion and dbt models, plan recovery and backfills, and address recurring failures.
- **Quality and observability:** maintain data contracts and schema checks, review run history, and tune actionable alerts.
- **Safe changes and handoffs:** review dependency upgrades and Terraform changes, strengthen CI checks, and keep runbooks and architecture decisions current.

An engagement starts by agreeing on the platform, ownership boundaries, backlog, and support expectations. Scope and response arrangements are agreed per engagement.

## Selected upstream documentation

| Contribution | Status | Operational detail |
| --- | --- | --- |
| [Airflow #71158](https://github.com/apache/airflow/pull/71158) | Merged | Distinguish metrics and traces in `otel_*` configuration |
| [Prefect #22533](https://github.com/PrefectHQ/prefect/pull/22533) | Merged | Global concurrency limit setup |
| [dbt docs #9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) | Merged | Use `duration_ms` for Fusion slowest-node ranking |
| [dbt docs #9960](https://github.com/dbt-labs/docs.getdbt.com/pull/9960) | Merged September 29, 2026 | Correct macro argument type to `bool` |

Statuses verified September 30, 2026. [Contribution record and current work](docs/work-history.md).

## Writing and contact

[Incremental loading and dbt](https://github.com/br413/br413.github.io/blob/main/articles/building-production-data-pipeline.md) · [Data quality contracts](https://github.com/br413/br413.github.io/blob/main/articles/data-quality-contracts-production-pipelines.md) · [Contract versioning](https://github.com/br413/br413.github.io/blob/main/articles/contract-versioning-production-pipelines.md)

For hiring or maintenance inquiries: **[br198064@gmail.com](mailto:br198064@gmail.com)**. Also available via [Telegram](https://t.me/CtrlAltBomb) or [WhatsApp](https://wa.me/12297421656).
