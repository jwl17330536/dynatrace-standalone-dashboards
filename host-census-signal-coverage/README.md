# Host Census + Signal Coverage

Monitors host fleet completeness and signal health by comparing the set of hosts Dynatrace knows about against the set actively reporting metrics. Surfaces hosts that have gone dark, hosts with missing or stale OneAgent, and gaps in signal coverage by group/tag.

## Artifacts

| File | Description |
|------|-------------|
| `host-census-signal-coverage.json` | Dashboard — fleet coverage tiles, signal dropout signals, missing agent coverage |
| `host-census-snapshot.workflow.json` | Scheduled workflow — daily snapshot of instrumented host set stored as a bizevent |
| `host-dropout-alert.workflow.json` | Alert workflow — opens a Dynatrace Problem after ~1 hour of silence from a previously reporting host |

## Prerequisites

- **Dynatrace OneAgent** deployed across your host fleet
- **Credential Vault entry** for the workflow API token (needs `metrics.read`, `problems.write`, `bizevents.ingest` scopes)

## Import

### Dashboard

1. Dynatrace → Dashboards → Import
2. Upload `host-census-signal-coverage.json`

### Workflows

1. Open each workflow JSON and replace the placeholder Vault ID with your own:
   ```
   CREDENTIALS_VAULT-REPLACE_WITH_YOUR_VAULT_ID
   ```
2. In `host-dropout-alert.workflow.json`, also set:
   ```
   DASHBOARD_ID = 'REPLACE_WITH_YOUR_DASHBOARD_ID'
   ```
   Use the ID of the dashboard you imported above (visible in the dashboard URL).
3. Dynatrace → Automations → Workflows → Import
4. Upload each workflow JSON

## How It Works

The **snapshot workflow** runs daily and stores a bizevent record of all instrumented hosts. The **alert workflow** compares the latest host set against the previous snapshot and opens a problem if any hosts drop out for more than ~1 hour. The **dashboard** visualizes current coverage, host signal health, and any active dropout alerts.
