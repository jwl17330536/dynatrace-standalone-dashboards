# NSLB / DNS Load Balancer

Monitors nslb (a DNS-based load balancer) alongside dnsdist health checks. Tracks freshness, CPU usage, health-check timeouts, and log volume — useful for validating that the load balancer is actively processing and routing queries.

## What it shows

- nslb-pi freshness (minutes since last log)
- dnsdist health-check timeouts
- nslb log line volume
- nslb CPU percentage (average)
- Health-check timeouts over time
- Log volume comparison (nslb vs. nslb-pi)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- nslb and dnsdist logs forwarded to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
