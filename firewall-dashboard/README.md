# Firewall Dashboard v4

Monitors a UniFi Dream Machine / UDM firewall alongside the AT&T BGW320 WAN edge. Tracks syslog ingest health, DNAT hits, content filter blocks, and WAN-side firewall activity — all parsed from syslog records forwarded to Dynatrace.

## What it shows

- UDM syslog ingest health (24h)
- DNAT hits over time
- Top external sources hitting DNAT rules
- Hits by service
- Content filter blocks
- BGW WAN blocks by reason

## Pre-requisites

- **Log Monitoring / Grail** enabled
- UDM/UDM Pro syslog forwarded to Dynatrace (via Bindplane or log forwarder)
- AT&T BGW320 syslog forwarded to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
