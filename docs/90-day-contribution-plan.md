# 90-day contribution plan

**Goal:** Build a credible, honest public data-engineering profile through consistent activity and upstream OSS merges — not backdated history.

**Started:** June 2026 · **Building in public since:** 2026  
**Review cadence:** Every 2 weeks

---

## North-star outcomes (Day 90)

| Outcome | Target |
|---------|--------|
| Upstream merged PRs (data platforms) | **5+** (Prefect, Airflow, dbt, Meltano) |
| Green contribution weeks | **10+ consecutive** |
| Portfolio releases | **v0.2.1** on `production-data-pipeline` (quarantine/DLQ) |
| Technical writing | **2** Dev.to articles |
| Pull Shark | Maintain Bronze; progress toward Silver organically |

---

## Weekly rhythm (repeat every week)

| Day | Activity | Time |
|-----|----------|------|
| **Mon** | Comment on 1 upstream issue; 1 small commit (docs/tests) on a portfolio repo | 30–45 min |
| **Wed** | OSS PR work or portfolio feature/fix | 1–2 hrs |
| **Fri** | README/ADR/ops runbook update; cross-link writing or portfolio | 30–45 min |

**Minimum bar:** 3 commit days per week across public repos.

---

## Phase 1 — Land in-flight work (Weeks 1–4)

### Week 1
- [x] Fix and merge **Prefect [#22533](https://github.com/PrefectHQ/prefect/pull/22533)** — P2 feedback addressed; awaiting maintainer re-review
- [x] Follow up on **Airflow [#70171](https://github.com/apache/airflow/pull/70171)** — rebased on main, CI fixes pushed (Aug 2026)
- [x] **Airflow [#70185](https://github.com/apache/airflow/pull/70185)** — closed per maintainer: wait for proper dbt Cloud OL facet ([#68661](https://github.com/apache/airflow/issues/68661))
- [x] Update profile README OSS table: mark **dbt [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606)** merged ✓

### Week 2
- [x] `production-data-pipeline`: add architecture diagram to README ([#28](https://github.com/br413/production-data-pipeline/pull/28))
- [x] Comment on **Airflow [#43366](https://github.com/apache/airflow/issues/43366)** before opening PR
- [x] Open **Airflow [#71158](https://github.com/apache/airflow/pull/71158)** — clarify metrics vs traces `otel_*` descriptions (approved by @ferruzzi)

### Week 3
- [x] `data-quality-observability`: add webhook integration test — [#9](https://github.com/br413/data-quality-observability/issues/9), PR [#10](https://github.com/br413/data-quality-observability/pull/10)

### Week 4
- [x] Comment on **Meltano [#6289](https://github.com/meltano/meltano/issues/6289)** — intent to add `elt` vs `run` docs
- [x] Open **Meltano [#10253](https://github.com/meltano/meltano/pull/10253)** — `elt` vs `run` decision guide in v2 migration docs
- [x] Release **production-data-pipeline v0.2.0** — [release](https://github.com/br413/production-data-pipeline/releases/tag/v0.2.0) published (changelog [#29](https://github.com/br413/production-data-pipeline/pull/29))
- [ ] Request indexing for new content in Google Search Console

---

## Phase 2 — Expand upstream footprint (Weeks 5–8)

### Week 5
- [x] Open PR for **Meltano [#6289](https://github.com/meltano/meltano/issues/6289)** — [#10253](https://github.com/meltano/meltano/pull/10253) opened (ahead of schedule)
- [x] Portfolio: add cost/ops notes to `cloud-lakehouse-blueprint` — [#6](https://github.com/br413/cloud-lakehouse-blueprint/pull/6)

### Week 6
- [x] Open PR for **dbt docs [#9717](https://github.com/dbt-labs/docs.getdbt.com/issues/9717)** — [#9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) (Fusion telemetry slowest-nodes example)
- [x] Release **production-data-pipeline v0.2.1** — [release](https://github.com/br413/production-data-pipeline/releases/tag/v0.2.1) (quarantine/DLQ)
- [x] Dev.to article #2: [*Data Quality Contracts in Production Pipelines*](https://dev.to/bobby_ray_581732c715283b2/data-quality-contracts-in-production-pipelines-without-a-separate-platform-team-f3) — published Aug 2026

### Week 7
- [x] `production-data-pipeline`: dead-letter / failed-record handling — design [#31](https://github.com/br413/production-data-pipeline/issues/31)/[#32](https://github.com/br413/production-data-pipeline/pull/32), implementation [#33](https://github.com/br413/production-data-pipeline/pull/33)
- [x] Review someone else's PR in Prefect or Airflow (comment only) — note on [Airflow #70400](https://github.com/apache/airflow/pull/70400)

### Week 8
- [x] Mid-plan retrospective: update OSS table and platform stack in profile README
- [ ] Target: **5th upstream merged PR** landed or in final review (4 open: Airflow #71158 approved, dbt #9781, Meltano #10253, Prefect #22533)

---

## Phase 3 — Consolidate reputation (Weeks 9–12)

### Week 9
- [x] Upstream follow-ups: merge bump **Airflow [#71158](https://github.com/apache/airflow/pull/71158)**, review nudge **dbt [#9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781)**, link **Meltano [#10253](https://github.com/meltano/meltano/pull/10253)** on [#6289](https://github.com/meltano/meltano/issues/6289), re-review **Prefect [#22533](https://github.com/PrefectHQ/prefect/pull/22533)**
- [x] Cross-link Dev.to article #2 from `production-data-pipeline` and `data-quality-observability` READMEs
- [x] Dev.to article #3 published: [*What I Learned Contributing to Prefect, dbt, and Airflow*](https://dev.to/bobby_ray_581732c715283b2/what-i-learned-contributing-to-prefect-dbt-and-airflow-an-honest-oss-retrospective-1ki8)
- [ ] Request GSC indexing — [article #2](https://dev.to/bobby_ray_581732c715283b2/data-quality-contracts-in-production-pipelines-without-a-separate-platform-team-f3), [article #3](https://dev.to/bobby_ray_581732c715283b2/what-i-learned-contributing-to-prefect-dbt-and-airflow-an-honest-oss-retrospective-1ki8), [br413.github.io](https://br413.github.io/)

### Week 10
- [x] `data-quality-observability`: schema registry / contract versioning design ADR — [#12](https://github.com/br413/data-quality-observability/pull/12) [ADR 0002](https://github.com/br413/data-quality-observability/blob/main/docs/adr/0002-schema-registry-and-contract-versioning.md), `contracts/registry.yml`
- [x] Apply learnings to portfolio README demos — full-stack / platform-stack demo sections in pipeline, quality, and lakehouse repos

### Week 11
- [ ] Small Airflow provider improvement (logging, docs, or test — not a mega-feature)
- [ ] Cross-link all repos from portfolio site Writing section

### Week 12
- [ ] Publish 90-day retrospective (Dev.to or GitHub discussion)
- [ ] Set next quarter targets (Silver Pull Shark is long-term; focus on quality merges)

---

## Next 5 upstream PR targets (prioritized)

| # | Repo | Target | Why | Status |
|---|------|--------|-----|--------|
| 1 | **Prefect** | [#22533](https://github.com/PrefectHQ/prefect/pull/22533) | Concurrency docs; P2 feedback addressed | Open — awaiting re-review |
| 2 | **Airflow** | [#70171](https://github.com/apache/airflow/pull/70171) | dbt Cloud failure details in task logs | Open — CI fixes pushed |
| 3 | **Airflow** | [#71158](https://github.com/apache/airflow/pull/71158) | Metrics vs traces `otel_*` config clarity | **Approved** — awaiting merge |
| 4 | **Meltano** | [#10253](https://github.com/meltano/meltano/pull/10253) | `elt` vs `run` docs; closes [#6289](https://github.com/meltano/meltano/issues/6289) | Open — awaiting review |
| 5 | **dbt docs** | [#9781](https://github.com/dbt-labs/docs.getdbt.com/pull/9781) | Fusion telemetry slowest-nodes fix; closes [#9717](https://github.com/dbt-labs/docs.getdbt.com/issues/9717) | Open — awaiting review |

**Already merged (keep on profile):**
- Prefect [#22500](https://github.com/PrefectHQ/prefect/pull/22500) ✓
- dbt docs [#9606](https://github.com/dbt-labs/docs.getdbt.com/pull/9606) ✓

---

## Rules (stay credible)

1. **Never backdate commits** — activity graph reflects real work only.
2. **Comment before PR** on upstream issues.
3. **Prefer data-platform repos** (dbt, Airflow, Prefect, Meltano) over unrelated forks.
4. **One meaningful merge beats five cosmetic self-PRs.**
5. **Profile, portfolio, and resume must agree.**

---

## Progress tracker

| Week | Dates | Commits | OSS PRs opened | OSS PRs merged | Notes |
|------|-------|---------|----------------|----------------|-------|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

_Update this table every Friday._
