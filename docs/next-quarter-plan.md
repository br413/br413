# Next quarter plan (September–November 2026)

**Follows:** [90-day-contribution-plan.md](./90-day-contribution-plan.md) · [90-day-retrospective.md](./90-day-retrospective.md)

**Theme:** Land in-flight upstream work, reduce WIP, deepen portfolio quality — not volume for badges.

---

## North-star outcomes (Day 180)

| Outcome | Target | Why |
|---------|--------|-----|
| Upstream merged PRs (cumulative) | **5+** | Close the gap from 2 → 5 with existing in-flight PRs first |
| Open upstream PRs at once | **≤ 2** | Review bandwidth is the bottleneck, not ideas |
| Portfolio milestone | **dqo v0.2** or pipeline **v0.3** | One release that closes an ADR phase |
| Technical writing | **1** focused article | Platform integration or contract versioning in production |
| Pull Shark | **Bronze maintained** | Silver is organic; no cosmetic self-PRs for badge chasing |

---

## Priority order (do not reorder casually)

### 1. Land existing upstream PRs

| PR | Action | Success criteria |
|----|--------|------------------|
| [Airflow #71158](https://github.com/apache/airflow/pull/71158) | Merge bump every 2 weeks | Merged |
| [Airflow #70171](https://github.com/apache/airflow/pull/70171) | Keep CI green after newsfragment fix | Merged or maintainer feedback addressed |
| [dbt docs #9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) | Review nudge monthly | Merged |
| [Meltano #10253](https://github.com/meltano/meltano/pull/10253) | Link on [#6289](https://github.com/meltano/meltano/issues/6289) when quiet | Review or merge |
| [Prefect #22533](https://github.com/PrefectHQ/prefect/pull/22533) | Re-review after P2 fixes | Merged |

**Rule:** No new upstream PR until at least one of the above merges.

### 2. Portfolio depth

| Repo | Milestone | Deliverable |
|------|-----------|-------------|
| [data-quality-observability](https://github.com/br413/data-quality-observability) | ADR 0002 phase 3 | Persist `contract_version` in run history; surface in `history` CLI |
| [production-data-pipeline](https://github.com/br413/production-data-pipeline) | v0.3.0 (optional) | Replay/quarantine metrics export or ops dashboard notes |
| [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint) | Maintenance | Keep ops runbook aligned with pipeline + dqo releases |

### 3. Visibility (manual)

- GSC indexing for all Dev.to articles and br413.github.io
- Dev.to cover images for articles #2 and #3
- Rotate Dev.to API key if exposed in chat logs

### 4. Writing (one article max)

**Candidate topic:** Contract versioning end-to-end — registry → CLI → Airflow DAG → run history (ties dqo ADR 0002 to production-data-pipeline quarantine story).

Draft ready: [articles/contract-versioning-production-pipelines.md](https://github.com/br413/br413.github.io/blob/main/articles/contract-versioning-production-pipelines.md) — publish with `.\scripts\publish-devto.ps1 -Article versioning` after review.

---

## Weekly rhythm (unchanged)

| Day | Activity | Time |
|-----|----------|------|
| **Mon** | Upstream follow-up comment + small portfolio commit | 30–45 min |
| **Wed** | OSS rebase/CI or portfolio feature | 1–2 hrs |
| **Fri** | Plan/README update, cross-links | 30–45 min |

**Minimum bar:** 3 public commit days per week.

---

## Monthly checkpoints

| Month | Check |
|-------|-------|
| **September** | #71158 merged; dqo phase 3 merged ([#14](https://github.com/br413/data-quality-observability/pull/14)); phase 4 CI guards ([#15](https://github.com/br413/data-quality-observability/pull/15)) |
| **October** | 2nd upstream merge landed (cumulative 4+); GSC complete |
| **November** | 5th cumulative merge OR honest closeout if blocked; next plan draft |

---

## Rules (carry forward)

1. Never backdate commits
2. Comment before PR on upstream issues
3. Prefer data-platform repos (dbt, Airflow, Prefect, Meltano)
4. One meaningful merge beats five cosmetic self-PRs
5. Profile, portfolio site, and resume must agree
6. No LinkedIn — GitHub, Dev.to, and portfolio site are the public channels

---

## Progress tracker (Q4)

| Month | Upstream merges | Portfolio releases | Articles | Notes |
|-------|-----------------|-------------------|----------|-------|
| Sep | | dqo ADR 0002 ph. 3–5; pipeline ADR 0005 | article #4 draft | ADR 0002 complete; [pipeline #37](https://github.com/br413/production-data-pipeline/pull/37) merged |
| Oct | | | | |
| Nov | | | | |

_Next phase: [nov-jan-contribution-plan.md](./nov-jan-contribution-plan.md) (Nov 2026 – Jan 2027)._

_Update on the first Friday of each month._
