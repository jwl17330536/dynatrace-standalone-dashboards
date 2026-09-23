# Home Automation Stack

Monitors a home automation stack running in Docker containers — covering Home Assistant, AppDaemon, and supporting services. Tracks container log volume, error rates, CPU usage, and log trends to detect unhealthy automation behavior.

## What it shows

- Container log line volume
- Home Assistant and AppDaemon error-ish log counts
- Host CPU percentage
- Log volume by container (time series)
- Container log volume trend over time

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Docker container logs forwarded to Dynatrace (via Bindplane or log forwarder)
- **OneAgent** on the host (for CPU metrics)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
