# Ansible Control Plane

Monitors an Ansible control plane node by parsing its log output. Tracks playbook run activity, error/failure rates, Git fetch operations, and overall log freshness — useful for validating that scheduled automation is running and healthy.

## What it shows

- Log line volume
- Log freshness (minutes since last entry)
- FAILED / FATAL / ERROR keyword counts
- Git and FETCH activity lines
- Log volume trend over time
- FAILED / FATAL / ERROR trend over time

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Ansible control node logs forwarded to Dynatrace

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
