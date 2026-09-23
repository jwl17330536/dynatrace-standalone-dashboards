# Netflow Traffic Analysis

Visualizes enriched NetFlow data to show where network traffic is going — by protocol, provider, country, port, and host pair. Designed for home lab and edge networks forwarding NetFlow records into Dynatrace via the Netflow & IPFIX extension.

## What it shows

- Total traffic volume and flow counts
- Protocol distribution (TCP, UDP, ICMP, etc.)
- Top providers by traffic volume (with ASN enrichment)
- Top ports by usage
- Top countries by traffic
- Top 50 host-pair conversations with enrichment (DNS, ASN, geo)

## Pre-requisites

- **Dynatrace Netflow & IPFIX extension** installed and receiving NetFlow records
- **Log Monitoring / Grail** enabled for DQL queries

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
