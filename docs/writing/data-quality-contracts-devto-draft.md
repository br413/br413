# Data Quality Contracts in Production Pipelines (Dev.to draft)

**Target:** Week 6 article #2 · cross-link [data-quality-observability](https://github.com/br413/data-quality-observability) + [production-data-pipeline](https://github.com/br413/production-data-pipeline)

---

## Title options

1. Data Quality Contracts in Production Pipelines (Without a Separate Platform Team)
2. From Schema Checks to Quarantine Tables: Layering Data Contracts in Python Pipelines

## Hook (first 2 sentences)

Production pipelines fail in two ways: loudly at 3 a.m., or quietly in the CEO's dashboard. Data quality contracts give you a third path — catch drift at the boundary, persist evidence, and route bad rows before they poison silver models.

## Outline

### 1. The problem: silent failure modes

- Schema drift lands in bronze; dbt tests fail downstream (or worse, pass on stale assumptions)
- One poison-pill API record aborts an entire ingestion page
- Operators grep logs instead of querying failure artifacts

### 2. What a contract is (and isn't)

- YAML contract: columns, null rules, freshness, referential integrity
- Not a replacement for warehouse-level tests — a **gate at the dataset boundary**
- Portfolio example: `data-quality-observability` contracts for orders/customers

```yaml
# Minimal example — link to repo
columns:
  - name: order_id
    type: string
    required: true
checks:
  - type: freshness
    max_age_hours: 24
```

### 3. Two layers in a real stack

| Layer | When | Project |
|-------|------|---------|
| **Row-level quarantine** | During ingestion | `production-data-pipeline` — invalid events → `bronze.quarantine_events` |
| **Dataset contracts** | After landing / before promote | `data-quality-observability` — run history + alerts |

Explain ADR 0004 quarantine decision: per-record routing, `records_quarantined` metric, dbt excludes quarantined IDs.

### 4. Alert routing that on-call will answer

- Console, JSONL file, webhook (`WebhookAlertChannel`)
- Ingestion webhooks: `zero_record_ingestion`, `ingestion_quarantine`
- Tie to operations runbooks — query quarantine table, replay procedure

### 5. CI as contract enforcement

- pytest for check logic + webhook mocks
- GitHub Actions runs contracts against sample CSV fixtures
- "Green CI" means the contract suite ran, not that production data is clean

### 6. Practical adoption path

1. Start with one high-value dataset contract (orders, events)
2. Add freshness + required-field checks before adding FK complexity
3. Add quarantine/DLQ when API sources are messy
4. Wire alerts to your existing webhook/Slack path

### 7. Closing + links

- [data-quality-observability](https://github.com/br413/data-quality-observability)
- [production-data-pipeline v0.2.1](https://github.com/br413/production-data-pipeline/releases/tag/v0.2.1) (quarantine)
- [Building a Production Data Pipeline…](https://dev.to/bobby_ray_581732c715283b2/building-a-production-data-pipeline-with-incremental-loading-and-dbt-2e2c) (article #1)

## Tags (Dev.to)

`dataengineering` `dbt` `python` `dataquality` `airflow`

## Checklist before publish

- [ ] Add one Mermaid diagram (bronze → quarantine vs bronze → silver)
- [ ] Screenshots: `python -m src.dqo.cli run` output + quarantine SQL query
- [ ] Cross-link from br413.github.io Writing section
- [ ] Request GSC indexing for new Dev.to URL
