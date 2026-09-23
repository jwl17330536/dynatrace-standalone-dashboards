# Netflow Network Analysis v2

Protocol and direction-level analysis of NetFlow traffic. Shows how traffic is distributed across TCP/UDP and other protocols over time, with totals for unique services and active source/destination IPs.

## What it shows

- Total data transferred and unique service count
- Active source and destination IP counts
- Traffic by protocol over time (time series)
- Traffic by direction over time (time series)

## Pre-requisites

- **Dynatrace Netflow & IPFIX extension** installed and receiving NetFlow records
- **Log Monitoring / Grail** enabled for DQL queries

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
