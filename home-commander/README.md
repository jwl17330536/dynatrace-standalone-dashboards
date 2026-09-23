# Home Commander v2

Monitors Home Commander, a home automation orchestration service that coordinates fleet sync, CMDB lookups, and workflow API calls. Tracks request rates, HTTP 5xx error rates, and host CPU — useful for validating that the orchestration layer is healthy.

## What it shows

- Nginx request volume
- Fleet sync, CMDB API, and workflow API hit counts
- HTTP 5xx-ish error count
- Host CPU percentage (average)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Nginx and application logs forwarded to Dynatrace
- **OneAgent** on the host (for CPU metrics)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
