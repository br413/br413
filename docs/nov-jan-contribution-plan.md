# November–January contribution plan (2026–2027)

**Follows:** [next-quarter-plan.md](./next-quarter-plan.md) (Sep–Nov 2026) · [90-day-retrospective.md](./90-day-retrospective.md)

**Theme:** Finish what is open, publish the versioning story, then reset WIP before any new upstream breadth.

---

## Starting position (end of Q4)

| Signal | Status |
|--------|--------|
| Upstream merges (cumulative) | **3** — Prefect #22500, dbt #9606, Airflow #71158 ✓ |
| In-flight upstream PRs | **5** — see priority table below |
| Portfolio | pipeline v0.2.1, dqo ADR 0002 complete, pipeline ADR 0005 pins |
| Writing | 3 Dev.to articles live; **article #4 draft ready** |
| Honest gap | Merge count below 5+ target; review bandwidth is the bottleneck |

---

## North-star outcomes (Jan 31, 2027)

| Outcome | Target | Why |
|---------|--------|-----|
| Upstream merged PRs (cumulative) | **5+** | Closes the gap from the 90-day plan |
| Open upstream PRs at once | **≤ 2** | Sustainable review load |
| Technical writing | **4** Dev.to articles | Article #4 publishes the registry → history story |
| Search visibility | GSC indexed | Articles #2–#4 + br413.github.io |
| Portfolio release | **pipeline v0.3.0** (optional) | Quarantine metrics or ops export — only if upstream is stable |
| Pull Shark | **Bronze maintained** | Silver is organic |

---

## Priority order

### 1. Land in-flight upstream (Nov–Dec)

| PR | Nov action | Dec action | Done when |
|----|------------|------------|-----------|
| [Airflow #71158](https://github.com/apache/airflow/pull/71158) | Merge bump (approved) | Escalate if stale 30+ days | Merged |
| [Airflow #70171](https://github.com/apache/airflow/pull/70171) | CI green; respond to review | Rebase if needed | Merged or closed gracefully |
| [dbt docs #9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) | Review nudge | Second nudge if quiet | Merged |
| [Meltano #10253](https://github.com/meltano/meltano/pull/10253) | Comment on [#6289](https://github.com/meltano/meltano/issues/6289) | Merge bump | Review or merge |
| [Prefect #22533](https://github.com/PrefectHQ/prefect/pull/22533) | Re-review request | Address any new feedback | Merged |

**Rules:**

- No **new** upstream PR until cumulative merges ≥ **3**
- After cumulative merges ≥ **5**, at most **one** new small docs/ops PR per month
- Close or withdraw stale PRs rather than let them rot

### 2. Publish article #4 (Dec)

Draft: [contract-versioning-production-pipelines.md](https://github.com/br413/br413.github.io/blob/main/articles/contract-versioning-production-pipelines.md)

```powershell
$env:DEVTO_API_KEY = "your-key"
.\scripts\publish-devto.ps1 -Article versioning
```

After publish:

- Add link to [br413.github.io](https://br413.github.io/) Writing section
- Update profile README Writing table
- Cross-link from pipeline + dqo READMEs
- Request GSC indexing

### 3. Visibility cleanup (Dec–Jan)

- [ ] GSC: articles #2, #3, #4, br413.github.io
- [ ] Dev.to cover images for articles #2, #3, #4
- [ ] Portfolio site Writing section lists article #4 + repo cross-links

### 4. Portfolio (Jan — optional)

Only if upstream WIP ≤ 2:

| Repo | Milestone | Deliverable |
|------|-----------|-------------|
| [production-data-pipeline](https://github.com/br413/production-data-pipeline) | v0.3.0 | Quarantine volume metrics in ops runbook or lightweight export |
| [data-quality-observability](https://github.com/br413/data-quality-observability) | Maintenance | Wire dqo into pipeline Airflow DAG post-dbt (stretch) |
| [cloud-lakehouse-blueprint](https://github.com/br413/cloud-lakehouse-blueprint) | Maintenance | Sync ops runbook with v0.3 if shipped |

---

## Monthly checkpoints

| Month | Must achieve | Stretch |
|-------|--------------|---------|
| **November 2026** | Q4 closeout doc updated; **#71158 merged** ✓ | 4th cumulative merge |
| **December 2026** | Article #4 published; GSC submitted for all URLs | 4th cumulative merge |
| **January 2027** | Honest Q1 retrospective; draft Feb–Apr plan | 5 cumulative merges; pipeline v0.3.0 |

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
| Nov 2026 | 3 | article #4 draft on site | | Airflow #71158 merged |
| Dec 2026 | | | | |
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
