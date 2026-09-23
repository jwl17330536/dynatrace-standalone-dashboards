# Dynatrace Standalone Dashboards

Standalone Dynatrace dashboards that visualize observability data without requiring any custom workflow. Each dashboard reads directly from Dynatrace's built-in data (OneAgent telemetry, RUM events, Grail) and can be imported as-is.

## Dashboards

| Folder | Dashboard | What it shows |
|--------|-----------|---------------|
| [oneagent-version-compliance/](oneagent-version-compliance/) | OneAgent Version Compliance | Installed OneAgent versions vs. baseline across all hosts |
| [rum-version-compliance/](rum-version-compliance/) | RUM Version Compliance v3 | RUM agent policy posture: on-target, below-target, unsupported, above-target |
| [rum-classic-js-versions/](rum-classic-js-versions/) | RUM Classic JS Versions | Latest RUM Classic JavaScript library versions per application |

## How to import a dashboard

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from the dashboard folder
4. The dashboard opens immediately — no configuration required

## Notes

- These dashboards do not depend on any workflow or custom automation.
- All data comes from Dynatrace's native telemetry (OneAgent, RUM, Grail).
- If a tile shows no data, confirm the relevant Dynatrace feature is enabled in your environment (see each dashboard's README).
