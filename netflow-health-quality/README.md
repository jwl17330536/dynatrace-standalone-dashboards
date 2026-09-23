# Netflow Health & Quality

Focused quality view that surfaces enrichment gaps, suspicious talkers, and unresolved DNS hotspots in the NetFlow pipeline. Use this alongside Netflow Diagnosis to identify which specific IPs or flows are dragging down data quality.

## What it shows

- Unknown direction percentage
- Top unenriched public IPs (ASN/geo enrichment gaps)
- Unresolved DNS hotspots by source and destination
- Suspicious talkers (inbound / outbound / low-confidence)
- Quality issue distribution

## Pre-requisites

- **Dynatrace Netflow & IPFIX extension** installed and receiving NetFlow records
- **Log Monitoring / Grail** enabled for DQL queries

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
