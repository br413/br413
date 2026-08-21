# What I Learned Merging PRs to Prefect, dbt, and Airflow (Dev.to draft)

**Target:** Week 9 article / GitHub Discussion · honest retrospective on upstream contribution experience

**Published articles (series):**
- [Building a Production Data Pipeline with Incremental Loading and dbt](https://dev.to/bobby_ray_581732c715283b2/building-a-production-data-pipeline-with-incremental-loading-and-dbt-2e2c)
- [Data Quality Contracts in Production Pipelines](https://dev.to/bobby_ray_581732c715283b2/data-quality-contracts-in-production-pipelines-without-a-separate-platform-team-f3)

---

## Title options

1. What I Learned Contributing Docs and Fixes to Prefect, dbt, and Airflow
2. Upstream PRs as a Senior Data Engineer: What Actually Gets Merged
3. From Portfolio Repos to Upstream Merges: A 90-Day OSS Retrospective

## Hook

Portfolio repos prove you can build. Upstream merges prove you can collaborate with teams that maintain the tools production platforms run on. This is what I learned doing both over 90 days — without backdating history or pretending employer work happened on GitHub.

## Outline

### 1. Why upstream, not just portfolio

- Hiring signal: judgment in someone else's codebase, not only greenfield demos
- Portfolio stack (pipeline + quality + lakehouse) gave **real context** for what to fix upstream
- Rule: comment on the issue before opening the PR

### 2. What merged (and why those landed)

| PR | Repo | Lesson |
|----|------|--------|
| [#22500](https://github.com/PrefectHQ/prefect/pull/22500) | Prefect | Ops detail (K8s readiness vs liveness) — small, verifiable, maintainer-aligned |
| [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606) | dbt docs | Troubleshooting for a deployment pitfall many teams hit silently |

**Pattern:** docs + operational clarity beat drive-by feature PRs for first contributions.

### 3. What's still open (and what that teaches)

| PR | Status | Lesson |
|----|--------|--------|
| Airflow [#71158](https://github.com/apache/airflow/pull/71158) | Approved — needs second reviewer | Large projects have merge policy, not just code quality |
| dbt [#9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) | Awaiting review | Issue-linked docs fixes still wait on maintainer bandwidth |
| Meltano [#10253](https://github.com/meltano/meltano/pull/10253) | Awaiting review | Tie PRs to maintainer-requested issues (#6289) |
| Prefect [#22533](https://github.com/PrefectHQ/prefect/pull/22533) | Changes requested → addressed | Automated review (P2) catches doc accuracy; respond precisely |
| Airflow [#70171](https://github.com/apache/airflow/pull/70171) | Open | Provider PRs need patience; keep CI green, don't churn |

### 4. What I would do differently

- **Fewer open PRs at once** — review bandwidth is the bottleneck after ~4 in flight
- **Airflow #70185** — closed when maintainer wanted proper OL facet; don't force the wrong abstraction
- **Rebase early** — Airflow moves fast; CI breaks if you wait weeks
- **Portfolio first, then upstream** — quarantine/DLQ in v0.2.1 made the data-quality article credible

### 5. The weekly rhythm that worked

- Mon: one upstream comment + one small portfolio commit
- Wed: OSS PR work or rebase/CI fix
- Fri: README/ADR cross-link or plan update

Minimum bar: 3 public commit days per week. Consistency beats hero days.

### 6. How portfolio and OSS reinforce each other

```text
production-data-pipeline (ingestion + quarantine)
    ↔ data-quality-observability (contracts)
    ↔ Dev.to articles (public narrative)
    ↔ upstream fixes (Prefect/Airflow/dbt/Meltano ops + docs)
```

Each layer answers a different reviewer question.

### 7. Closing + honest scorecard

- Merges landed: 2 (target was 5+ — still in progress)
- Dev.to articles: 2 ✓
- Portfolio release: v0.2.1 ✓
- Credibility rule: never backdate; profile, portfolio, and resume must agree

Links: [br413.github.io](https://br413.github.io/) · [90-day plan](../90-day-contribution-plan.md) · [GitHub profile](https://github.com/br413)

## Tags (Dev.to)

`dataengineering` `opensource` `career` `airflow`

## Checklist before publish

- [ ] Include honest merge count (don't inflate)
- [ ] No employer-confidential details
- [ ] Cross-link from br413.github.io Writing section
- [ ] Request GSC indexing after publish
