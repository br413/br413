# 90-day contribution retrospective (June–August 2026)

**Author:** [br413](https://github.com/br413) · **Plan:** [90-day-contribution-plan.md](https://github.com/br413/br413/blob/main/docs/90-day-contribution-plan.md)

This is the closeout scorecard for the first ninety-day push to build a credible, honest public data-engineering profile. For OSS-specific lessons (what merged, what stalled, weekly rhythm), see the Dev.to article [*What I Learned Contributing to Prefect, dbt, and Airflow*](https://dev.to/bobby_ray_581732c715283b2/what-i-learned-contributing-to-prefect-dbt-and-airflow-an-honest-oss-retrospective-1ki8).

---

## North-star outcomes (final)

| Outcome | Target | Result | Notes |
|---------|--------|--------|-------|
| Upstream merged PRs (data platforms) | **5+** | **2** | Prefect [#22500](https://github.com/PrefectHQ/prefect/pull/22500), dbt docs [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606) |
| Green contribution weeks | **10+ consecutive** | **~12** | Mon/Wed/Fri rhythm held across portfolio + upstream |
| Portfolio releases | **v0.2.1** quarantine/DLQ | **✓** | [production-data-pipeline v0.2.1](https://github.com/br413/production-data-pipeline/releases/tag/v0.2.1) |
| Technical writing | **2** Dev.to articles | **3** ✓ | Bonus OSS retrospective (article #3) |
| Pull Shark | Maintain Bronze; progress toward Silver | **Bronze** | Silver is long-term; quality merges over volume |

**Honest gap:** The merge count missed the 5+ target. Four PRs remain in active review ([Airflow #71158](https://github.com/apache/airflow/pull/71158) approved, [#70171](https://github.com/apache/airflow/pull/70171), [dbt #9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781), [Meltano #10253](https://github.com/meltano/meltano/pull/10253), [Prefect #22533](https://github.com/PrefectHQ/prefect/pull/22533)). That is normal for large upstream projects — the work is real and maintained, not abandoned drive-bys.

---

## What shipped

### Portfolio stack

| Repo | Highlights |
|------|------------|
| [production-data-pipeline](https://github.com/br413/production-data-pipeline) | v0.2.0 → v0.2.1, quarantine/DLQ ([ADR 0004](https://github.com/br413/production-data-pipeline/blob/main/docs/adr/0004-dead-letter-quarantine.md)), architecture diagram, full-stack demo |
| [data-quality-observability](https://github.com/br413/data-quality-observability) | Webhook integration tests, [ADR 0002](https://github.com/br413/data-quality-observability/blob/main/docs/adr/0002-schema-registry-and-contract-versioning.md) schema registry, CLI `--contract orders` resolution |
| [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint) | Ops runbook, cost notes, platform-stack cross-links |
| [lakehouse-platform-starter](https://github.com/br413/lakehouse-platform-starter) | Flagship reference architecture (pinned) |
| [br413.github.io](https://br413.github.io/) | OSS table synced, Writing section with repo cross-links |

### Writing

1. [Building a Production Data Pipeline with Incremental Loading and dbt](https://dev.to/bobby_ray_581732c715283b2/building-a-production-data-pipeline-with-incremental-loading-and-dbt-2e2c)
2. [Data Quality Contracts in Production Pipelines](https://dev.to/bobby_ray_581732c715283b2/data-quality-contracts-in-production-pipelines-without-a-separate-platform-team-f3)
3. [What I Learned Contributing to Prefect, dbt, and Airflow](https://dev.to/bobby_ray_581732c715283b2/what-i-learned-contributing-to-prefect-dbt-and-airflow-an-honest-oss-retrospective-1ki8)

### Upstream (merged)

- **Prefect #22500** — Kubernetes readiness vs liveness probes
- **dbt docs #9606** — Prefixed custom schema troubleshooting

### Upstream (in flight at closeout)

- **Airflow #71158** — Approved; metrics vs traces `otel_*` clarity
- **Airflow #70171** — dbt Cloud failure details in task logs (newsfragment CI fixed Week 11)
- **dbt docs #9781** — Fusion telemetry `duration_ms` fix
- **Meltano #10253** — `elt` vs `run` decision guide
- **Prefect #22533** — Concurrency docs (P2 feedback addressed)

**Closed gracefully:** Airflow [#70185](https://github.com/apache/airflow/pull/70185) — maintainer wanted proper dbt Cloud OL facet instead.

---

## What worked

1. **Portfolio first, then upstream narrative** — shipping quarantine/DLQ made the contracts article credible
2. **Issue-linked, small PRs** — docs and ops clarity merged faster than feature work
3. **Mon/Wed/Fri rhythm** — three public commit days per week beat hero sprints
4. **Single source of truth** — profile README, portfolio site, and plan stayed aligned
5. **Honest scorecard** — stating the merge gap plainly is more credible than inflating it

## What I would change next time

1. **Cap open upstream PRs at 3** — review bandwidth became the bottleneck after four in flight
2. **Rebase within 48 hours** on Airflow — upstream moves fast; stale branches break CI
3. **GSC indexing same week as publish** — search visibility lagged because indexing stayed manual
4. **One upstream repo at a time until first merge** — depth before breadth for initial credibility

---

## Manual items still open

- [ ] Google Search Console indexing for [article #2](https://dev.to/bobby_ray_581732c715283b2/data-quality-contracts-in-production-pipelines-without-a-separate-platform-team-f3), [article #3](https://dev.to/bobby_ray_581732c715283b2/what-i-learned-contributing-to-prefect-dbt-and-airflow-an-honest-oss-retrospective-1ki8), [br413.github.io](https://br413.github.io/)
- [ ] Dev.to cover images for articles #2 and #3

---

## Next quarter

See **[next-quarter-plan.md](https://github.com/br413/br413/blob/main/docs/next-quarter-plan.md)** — focus on landing in-flight merges, reducing WIP, and one portfolio milestone (dqo contract versioning phase 3).

---

*Building in public since 2026. No backdated commits. Profile, portfolio, and writing agree.*
