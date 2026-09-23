# Netflow Operations Health v2

Monitors the operational health and data quality of your NetFlow pipeline. Tracks enrichment coverage, DNS resolution rates, and a composite data quality score — essential for understanding whether your NetFlow data can be trusted for analysis.

## What it shows

- Unknown direction percentage
- DNS resolution issues percentage
- Unenriched IP percentage (ASN/geo gaps)
- Composite data quality score
- Data quality trend over time
- Top unknown-direction sources

## Pre-requisites

- **Dynatrace Netflow & IPFIX extension** installed and receiving NetFlow records
- **Log Monitoring / Grail** enabled for DQL queries

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
