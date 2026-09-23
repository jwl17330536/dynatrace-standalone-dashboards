# Network Overview v3

Master landing page for home network observability. Aggregates key signals from BGW broadband, UniFi clients, NetFlow, DNS, and open problems into a single view — designed as a quick-glance health board across the full network stack.

## What it shows

- BGW broadband status
- Active UniFi client count
- NetFlow flow count
- DNS unresolved percentage
- Open problems across network entities
- BGW firewall spike detection (blocks per 5 minutes)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Netflow & IPFIX extension, UniFi syslog, BGW syslog, and DNS logs forwarded to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
