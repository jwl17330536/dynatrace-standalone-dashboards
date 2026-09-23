# Observability Health Dashboard

Version history of an Observability Health Dashboard tracking application observability posture and CMDB coverage. Three versions are included in this folder representing different generations of the dashboard.

| File | Version | Notes |
|---|---|---|
| `observability-health-dashboard.json` | Base (original) | CMDB and application coverage view |
| `observability-health-dashboard.v8.json` | v8 | Expanded problem and entity coverage |
| `observability-health-dashboard.v10.json` | v10 | Current production version |

## What it shows

- Active and total problems by application
- CMDB server and application counts
- Application coverage by tier
- Monitored entity summary

## Pre-requisites

- **Grail** enabled for DQL queries on problems and entities
- CMDB sync workflow configured (for CMDB-sourced tiles)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file for the version you want to use
4. The dashboard opens immediately
