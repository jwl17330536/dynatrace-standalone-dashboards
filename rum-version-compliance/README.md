# RUM Version Compliance

Classifies RUM applications by their JavaScript agent policy status: on-target, below-target, unsupported, and above-target. Designed for operations and enablement teams who need to see RUM version posture at a glance and prioritize remediation.

## What it shows

- Per-application RUM agent version classification
- Policy compliance summary (on-target vs. drift)
- Applications flagged as below-target or on unsupported versions

## Pre-requisites

- **RUM (Real User Monitoring)** enabled in your Dynatrace environment
- **Grail** enabled (the dashboard uses DQL `fetch events`)
- RUM applications instrumented with the Dynatrace JavaScript agent (OneAgent injection or manual tag)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload `rum-version-compliance-dashboard.v3.json`
4. The dashboard opens immediately

> **Note:** The dashboard JSON has `isPrivate: true`, so after import it will only be visible to you. To share it with your team, open the dashboard, click the share icon, and update the visibility settings.

## Configuration

No manual configuration is required. The dashboard reads directly from RUM telemetry events in Grail.

If tiles show no data:
- Confirm RUM is enabled: **Settings** → **RUM** → ensure JavaScript agent injection is active
- Confirm your applications have recent user sessions (last 7 days by default)
- Check that Grail data retention covers the selected time range

## Data sources

| Tile | Source |
|------|--------|
| Application version list | `fetch events` — RUM agent version events |
| Compliance classification | `fetch events` — policy-evaluated RUM telemetry |
