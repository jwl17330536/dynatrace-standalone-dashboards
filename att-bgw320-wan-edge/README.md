# AT&T BGW320 / WAN Edge v4

Monitors the AT&T BGW320 residential gateway and WAN edge — including broadband status, GPON optical power levels, firewall block activity, and WAN receive bytes. Data is sourced from syslog and SNMP metrics forwarded to Dynatrace.

## What it shows

- Broadband status
- Firewall blocks by protocol
- GPON Rx / Tx optical power (dBm)
- WAN receive bytes (cumulative)
- BGW firewall vs. UniFi WAN event comparison
- Open problems on BGW-related entities

## Pre-requisites

- **Log Monitoring / Grail** enabled
- AT&T BGW320 syslog forwarded to Dynatrace
- SNMP metrics collection configured for the BGW320

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
