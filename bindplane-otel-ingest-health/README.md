# Bindplane / OTel Ingest Health

Monitors the health of a Bindplane-managed OpenTelemetry log ingest pipeline. Tracks collector log volume, error/warning rates, OTLP ingest line counts, edge host coverage, and per-host breakdowns — essential for validating that your OTel collectors are active and forwarding data.

## What it shows

- Collector log line volume
- OTLP ingest line count
- OTLP edge host count
- Collector error / warning line count
- Collector log volume by host (time series)
- OTLP ingest by host (time series)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Bindplane-managed OTel collectors deployed and forwarding logs to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
