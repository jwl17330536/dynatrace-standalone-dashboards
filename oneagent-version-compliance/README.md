# OneAgent Version Compliance

Shows installed OneAgent versions across all monitored hosts and compares them against the latest available release baseline. Useful for platform teams tracking version drift and planning upgrades.

## What it shows

- Current OneAgent version distribution across hosts
- Which hosts are on the latest, previous, or outdated releases
- Baseline version data collected by a companion workflow (if configured)

## Pre-requisites

- **OneAgent deployed** on hosts in your Dynatrace environment
- **Grail** enabled (the dashboard uses DQL `fetch dt.entity.host` and `fetch events`)
- **Optional — baseline workflow**: The baseline comparison tiles read from `OneAgentBaseline|<latest>|<oldest>|<fetched_at>` events produced by the `oneagent-baseline-sync` workflow. Without it, only live host data tiles will populate; the baseline comparison tiles will be empty.

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload `oneagent-version-dashboard.json`
4. The dashboard opens immediately

## Configuration

No configuration is required for the live host version tiles. If you want the baseline comparison tiles to populate:

1. Deploy the `oneagent-baseline-sync` workflow (available in the `references/` folder of `dynatrace-version-release-tracking`)
2. Run it once manually to seed the baseline events
3. The comparison tiles will populate on the next dashboard load

## Data sources

| Tile | Source |
|------|--------|
| Host version distribution | `fetch dt.entity.host` via DQL |
| Version compliance status | `fetch events` — live OneAgent telemetry |
| Baseline comparison | `fetch events` — `OneAgentBaseline|*` events from companion workflow |
