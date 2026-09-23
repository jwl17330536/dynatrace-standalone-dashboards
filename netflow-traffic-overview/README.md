# Netflow Traffic Overview

High-level summary of NetFlow ingest health and traffic direction. Useful as a quick-glance view of NetFlow volume, unique hosts, and data quality status before diving into deeper analysis dashboards.

## What it shows

- Total traffic volume and flow count
- Unique hosts seen
- Unknown direction percentage (data quality indicator)
- Traffic by direction over time (inbound / outbound / internal)
- Traffic by provider over time (enriched view)

## Pre-requisites

- **Dynatrace Netflow & IPFIX extension** installed and receiving NetFlow records
- **Log Monitoring / Grail** enabled for DQL queries

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
