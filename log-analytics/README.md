# Log Analytics

General-purpose log analytics dashboard covering log status distribution, top log messages, trace-connected error logs, and log sources. Useful as an entry point for log investigation across any Dynatrace environment with Grail log ingestion.

## What it shows

- Logs per status over time (with sums per status)
- Top 20 log messages overall
- Top 20 log messages for selected status
- Top 20 log messages for selected status connected to a trace
- Top log sources
- NONE-status logs with error-level content

## Pre-requisites

- **Log Monitoring / Grail** enabled with logs ingested into the environment

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
