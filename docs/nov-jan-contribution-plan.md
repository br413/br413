# November–January contribution plan (2026–2027)

**Follows:** [next-quarter-plan.md](./next-quarter-plan.md) (Sep–Nov 2026) · [90-day-retrospective.md](./90-day-retrospective.md)

**Theme:** Finish what is open, publish the versioning story, then reset WIP before any new upstream breadth.

---

## Starting position (end of Q4)

| Signal | Status |
|--------|--------|
| Upstream merges (cumulative) | **5** — Prefect #22500, dbt #9606, Airflow #71158, dbt docs #9781, Meltano #10253 ✓ |
| In-flight upstream PRs | **2** tracked — Airflow #70171, Prefect #22533 |
| Portfolio | pipeline **v0.3.0** ✓, dqo ADR 0002 complete, pipeline ADR 0005 pins |
| Writing | **4** Dev.to articles live — [article #4](https://dev.to/bobby_ray_581732c715283b2/contract-versioning-in-production-pipelines-registry-cli-and-run-history-13el) published Aug 2026 |
| Honest gap | 5+ merge target met; remaining WIP is review bandwidth |

---

## North-star outcomes (Jan 31, 2027)

| Outcome | Target | Why |
|---------|--------|-----|
| Upstream merged PRs (cumulative) | **5+** ✓ | Closes the gap from the 90-day plan |
| Open upstream PRs at once | **≤ 2** | Sustainable review load |
| Technical writing | **4** Dev.to articles | Article #4 publishes the registry → history story |
| Search visibility | GSC indexed | Articles #2–#4 + br413.github.io |
| Portfolio release | **pipeline v0.3.0** ✓ | [v0.3.0 release](https://github.com/br413/production-data-pipeline/releases/tag/v0.3.0) — quarantine metrics CLI |
| Pull Shark | **Bronze maintained** | Silver is organic |

---

## Priority order

### 1. Land in-flight upstream (Nov–Dec)

| PR | Nov action | Dec action | Done when |
|----|------------|------------|-----------|
| [Airflow #71158](https://github.com/apache/airflow/pull/71158) | ~~Merge bump~~ | — | **Merged** ✓ |
| [Airflow #70171](https://github.com/apache/airflow/pull/70171) | CI green; respond to review | Rebase if needed | Merged or closed gracefully |
| [dbt docs #9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) | ~~Review nudge~~ | — | **Merged** ✓ |
| [Meltano #10253](https://github.com/meltano/meltano/pull/10253) | Relocate + `el` vs deprecated `elt` ✓ | — | **Merged** ✓ |
| [Prefect #22533](https://github.com/PrefectHQ/prefect/pull/22533) | Re-review request | Address any new feedback | Merged |

**Rules:**

- No **new** upstream PR until cumulative merges ≥ **3**
- After cumulative merges ≥ **5**, at most **one** new small docs/ops PR per month
- Close or withdraw stale PRs rather than let them rot

### 2. Publish article #4 — done ✓

Published: [Contract Versioning in Production Pipelines](https://dev.to/bobby_ray_581732c715283b2/contract-versioning-in-production-pipelines-registry-cli-and-run-history-13el) (Aug 2026). Site and README cross-links synced.

### 3. Visibility cleanup (Dec–Jan)

- [ ] Request GSC indexing (articles #2–#4 + br413.github.io)
- [ ] Dev.to cover image for article #4 (and #2–#3 if missing)

### 4. Portfolio (Jan — optional)

Only if upstream WIP ≤ 2:

| Repo | Milestone | Deliverable |
|------|-----------|-------------|
| [production-data-pipeline](https://github.com/br413/production-data-pipeline) | **v0.3.0** ✓ | [Quarantine volume metrics](https://github.com/br413/production-data-pipeline/releases/tag/v0.3.0) — CLI + ops runbook |
| [data-quality-observability](https://github.com/br413/data-quality-observability) | Maintenance | Wire dqo into pipeline Airflow DAG post-dbt (stretch) |
| [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint) | Maintenance | Sync ops runbook with v0.3 if shipped |

---

## Monthly checkpoints

| Month | Must achieve | Stretch |
|-------|--------------|---------|
| **November 2026** | Q4 closeout doc updated; **#71158 merged** ✓ | 4th cumulative merge |
| **December 2026** | GSC submitted for all URLs; cover images | 4th cumulative merge |
| **January 2027** | Honest Q1 retrospective; draft Feb–Apr plan | ~~5 cumulative merges~~ ✓; ~~pipeline v0.3.0~~ ✓ |

---

## Weekly rhythm (unchanged)

| Day | Activity | Time |
|-----|----------|------|
| **Mon** | Upstream follow-up + small portfolio commit | 30–45 min |
| **Wed** | OSS rebase/CI or portfolio feature | 1–2 hrs |
| **Fri** | Plan/README/site cross-links | 30–45 min |

**Minimum bar:** 3 public commit days per week.

---

## Progress tracker

| Month | Upstream merges (cum.) | Articles | GSC | Notes |
|-------|------------------------|----------|-----|-------|
| Nov 2026 | **5** | 4 live | | [Meltano #10253](https://github.com/meltano/meltano/pull/10253) merged; #9781; #71158; [pipeline v0.3.0](https://github.com/br413/production-data-pipeline/releases/tag/v0.3.0) |
| Dec 2026 | | 4 live | pending | Article #4 published early (Aug) |
| Jan 2027 | | | | |

_Update on the first Friday of each month._

---

## Rules (carry forward)

1. Never backdate commits
2. Comment before PR on upstream issues
3. Prefer data-platform repos (dbt, Airflow, Prefect, Meltano)
4. One meaningful merge beats five cosmetic self-PRs
5. Profile, portfolio site, and writing must agree
6. GitHub, Dev.to, and br413.github.io are the public channels

---

## Q1 closeout (last week of January)

Publish a short update in [GitHub Discussions](https://github.com/br413/br413/discussions) or extend the profile plan:

- Cumulative merge count (honest)
- Article #4 link
- What blocked merges (if any)
- Feb–Apr targets (likely: maintain ≤2 WIP, one portfolio release, zero badge chasing)
