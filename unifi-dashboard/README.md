# UniFi Dashboard v3

Monitors a UniFi network environment — including active clients, WAN status, ISP information, internet disruption events, and syslog ingest health. Data is sourced from UniFi syslog records forwarded to Dynatrace.

## What it shows

- Active client count
- Active WAN and ISP status
- WAN events over the last 7 days
- Internet down / restored events by WAN
- Syslog ingest health (24h)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- UniFi controller syslog forwarded to Dynatrace (via Bindplane or log forwarder)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
