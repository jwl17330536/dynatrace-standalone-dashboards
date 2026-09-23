# Alert Volume Reduction

Analyzes Dynatrace problem and Davis event history to identify alert volume hotspots and track reduction efforts. Helps platform and SRE teams prioritize which problem sources to tune, suppress, or resolve to reduce noise.

## What it shows

- Total problems and Davis events
- Active problems now
- Average resolution time
- Top 20 problems by count (last 30 days)
- Problems by category

## Pre-requisites

- **Grail** enabled for DQL queries on `fetch dt.davis.problems` and `fetch dt.davis.events`

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
