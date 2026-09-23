# DNS v4

Monitors a self-hosted DNS infrastructure built on BIND and dnsdist. Tracks query volume by host, top queried names, health check issues, and log freshness — useful for home lab or edge DNS operators running Dynatrace Log Monitoring.

## What it shows

- DNS host usage distribution
- Latest queries
- dnsdist health check issues
- dnsdist log volume by host
- BIND log freshness (minutes)
- Top queried names (ns1)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- BIND and dnsdist logs forwarded to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
