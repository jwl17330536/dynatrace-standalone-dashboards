# Environment Overview - v1

Top-level environment health dashboard showing the current state of problems, log errors, traces, and monitored hosts. Designed as a starting-point overview for any Dynatrace environment.

## What it shows

- Open problems now
- Log volume — errors, warnings, and critical (stacked)
- Span response time — p50, p95, p99
- Top log error sources (last 1 hour)
- Problems over the last 24 hours
- Monitored host count

## Pre-requisites

- **Grail** enabled for DQL queries on logs, spans, and problems
- **OneAgent** deployed on hosts (for host count)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
