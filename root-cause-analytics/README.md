# Root Cause Analytics

Parameterized analytics dashboard for exploring Dynatrace problem history by entity tag. Uses dashboard variables to slice problems by tag key and event name — showing problem frequency, root cause percentages, capacity savings, and digital disruption avoided.

## What it shows

- Problems per day
- Problem types and root cause percentage by tag
- Resource capacity savings
- Digital disruption avoided
- Top entities for the selected tag and event type
- Comparison to previous 30-day period

## Pre-requisites

- **Grail** enabled for DQL queries on `fetch dt.davis.problems`
- Entities tagged consistently in your environment (used by dashboard variables `$tagKey` and `$eventName`)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
