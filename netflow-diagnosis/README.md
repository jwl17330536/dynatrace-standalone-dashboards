# Netflow Diagnosis

Deep-dive diagnostic dashboard for troubleshooting NetFlow data quality issues. Surfaces hotspots where flows are missing direction, DNS resolution is failing, or IPs lack ASN enrichment — used to identify configuration gaps in the NetFlow pipeline.

## What it shows

- Unknown direction, unresolved DNS, and unenriched public IP percentages
- Low-confidence direction percentage
- Flow volume vs. quality issues over time
- Unknown direction hotspots (source/destination breakdown)

## Pre-requisites

- **Dynatrace Netflow & IPFIX extension** installed and receiving NetFlow records
- **Log Monitoring / Grail** enabled for DQL queries

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
