# Audit Logs Time Analysis

Explores Dynatrace audit log data with time-series breakdowns. Contains a high-density tile layout for analyzing audit log events across the environment.

## What it shows

- Audit log events over time (multi-tile time series and categorical views)

## Pre-requisites

- **Grail** enabled for DQL queries on `fetch dt.system.audit_logs`
- Appropriate audit log access permissions in your Dynatrace environment

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
