# Home Ops Master Landing v12

Master landing dashboard for a full home operations stack built on Dynatrace. Aggregates signal freshness, ingest health, active host counts, open problems, and RUM coverage across the entire home infrastructure — used as the daily driver ops view.

## What it shows

- RUM app last-seen coverage (7d sparse apps)
- BGW poller, NetFlow, and OTLP ingest freshness (minutes)
- OneAgent active host count (2h window)
- OTLP/Pi log host count (24h)
- Open problems (excluding kiosk noise)
- Per-system health tiles across network, home automation, and infrastructure

## Pre-requisites

- Full home observability stack: OneAgent, Log Monitoring / Grail, Netflow extension, UniFi syslog, BGW syslog, RUM, Bindplane OTel
- Multiple companion dashboards for drill-down (NetFlow, Home Automation, UniFi, etc.)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
