# HAProxy Ingest Health (utility29)

Tracks the health of a HAProxy instance running on a Proxmox node (utility29) used as an OTLP front-end for log and metric ingest. Shows log volume, error/warning rates, freshness, and backend keyword activity.

## What it shows

- OTLP log line volume (utility29)
- Ingest freshness (minutes since last log)
- HAProxy keyword hits (errors, backend issues)
- haproxy.log lines since last deploy
- Log volume trend by host
- Backend / server keyword breakdown

## Pre-requisites

- **Log Monitoring / Grail** enabled
- HAProxy logs forwarded to Dynatrace from utility29

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
