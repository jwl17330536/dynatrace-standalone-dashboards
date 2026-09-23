# Proxmox Cluster

Monitors a Proxmox VE homelab cluster by parsing pveproxy and API extension logs. Tracks node activity, log freshness, API extension health, and per-node CPU usage for NUC-class nodes in the cluster.

## What it shows

- pveproxy log line volume
- API extension log line volume
- Extension freshness (minutes since last log)
- NUC hosts seen
- pveproxy volume by node (time series)
- NUC node CPU usage

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Proxmox pveproxy and API logs forwarded to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
