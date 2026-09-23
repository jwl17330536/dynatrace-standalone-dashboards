# RUM Classic JS Versions

Shows the latest RUM Classic JavaScript library versions in use across applications, along with sync status and run summary metrics. Useful for teams validating RUM Classic instrumentation consistency before migrating to newer agent versions.

## What it shows

- Latest Classic JS library version per application
- Sync status across applications
- Run summary metrics for Classic JS instrumentation

## Pre-requisites

- **RUM Classic** (Classic JavaScript injection) configured for one or more applications in your Dynatrace environment
- **Grail** enabled (the dashboard uses DQL `fetch events`)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload `rum-classic-js-version-dashboard.json`
4. The dashboard opens immediately

## Configuration

No manual configuration is required. The dashboard reads directly from RUM Classic telemetry in Grail.

If tiles show no data:
- Confirm Classic JS agent injection is enabled: **Settings** → **RUM** → **JavaScript agent**
- Confirm your applications have active Classic JS instrumentation (not OneAgent auto-injection)
- Verify recent user sessions exist in the selected time range

## Data sources

| Tile | Source |
|------|--------|
| JS library versions | `fetch events` — RUM Classic JS version events |
| Sync status | `fetch events` — instrumentation sync telemetry |

## Note on Classic vs. Modern RUM

Dynatrace offers both Classic JavaScript injection and the newer OneAgent-based RUM injection. This dashboard covers the Classic variant. For modern RUM version posture, see `rum-version-compliance/`.
