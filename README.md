# Dynatrace Standalone Dashboards

Standalone Dynatrace dashboards that visualize observability data without requiring any custom workflow. Each dashboard reads directly from Dynatrace's built-in data (OneAgent telemetry, RUM events, Grail, logs) and can be imported as-is.

## How to import a dashboard

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from the dashboard folder
4. The dashboard opens immediately — no configuration required beyond what each README notes

## Notes

- These dashboards do not depend on any workflow or custom automation unless noted.
- All data comes from Dynatrace's native telemetry (OneAgent, RUM, Grail, Log Monitoring).
- If a tile shows no data, confirm the relevant Dynatrace feature is enabled in your environment (see each dashboard's README).

---

## Dashboards

### Dynatrace Platform

| Folder | Dashboard | What it shows |
|--------|-----------|---------------|
| [oneagent-version-compliance/](oneagent-version-compliance/) | OneAgent Version Compliance | Installed OneAgent versions vs. baseline across all hosts |
| [rum-version-compliance/](rum-version-compliance/) | RUM Version Compliance v3 | RUM agent policy posture: on-target, below-target, unsupported, above-target |
| [rum-classic-js-versions/](rum-classic-js-versions/) | RUM Classic JS Versions | Latest RUM Classic JavaScript library versions per application |
| [host-census-signal-coverage/](host-census-signal-coverage/) | Host Census + Signal Coverage v3 | Host inventory and signal coverage across the estate |
| [environment-overview/](environment-overview/) | Environment Overview - v1 | Open problems, log errors, trace latency, and monitored host count |
| [observability-health-dashboard/](observability-health-dashboard/) | Observability Health Dashboard (v1 / v8 / v10) | Application observability posture and CMDB coverage — three versions |
| [dynatrace-assist-operator-cost/](dynatrace-assist-operator-cost/) | Dynatrace Assist — Operator Utilization & Cost | Operator skill usage by user, billed bytes, and conversation sessions |
| [alert-volume-reduction/](alert-volume-reduction/) | Alert Volume Reduction | Problem and Davis event volume analysis for noise reduction |
| [root-cause-analytics/](root-cause-analytics/) | Root Cause Analytics | Problem frequency and root cause percentage sliced by entity tag |
| [log-analytics/](log-analytics/) | Log Analytics | Log status distribution, top messages, and trace-connected error logs |
| [aws-cost-optimization/](aws-cost-optimization/) | AWS Cost Optimization | Underutilized EC2 instances and idle EBS volumes for rightsizing |

### Netflow / Network Traffic

| Folder | Dashboard | What it shows |
|--------|-----------|---------------|
| [netflow-traffic-overview/](netflow-traffic-overview/) | Netflow Traffic Overview | High-level NetFlow ingest health, flow count, and traffic direction |
| [netflow-traffic-analysis/](netflow-traffic-analysis/) | Netflow Traffic Analysis | Traffic by protocol, provider, country, port, and host-pair conversations |
| [netflow-network-analysis/](netflow-network-analysis/) | Netflow Network Analysis v2 | Protocol and direction breakdown with unique service and IP counts |
| [netflow-health-quality/](netflow-health-quality/) | Netflow Health & Quality | Enrichment gaps, suspicious talkers, and DNS resolution hotspots |
| [netflow-operations-health/](netflow-operations-health/) | Netflow Operations Health v2 | Composite data quality score and enrichment coverage trends |
| [netflow-diagnosis/](netflow-diagnosis/) | Netflow Diagnosis | Deep-dive into unknown direction, DNS, and enrichment failure hotspots |

### Network / Infrastructure

| Folder | Dashboard | What it shows |
|--------|-----------|---------------|
| [network-overview/](network-overview/) | Network Overview v3 | Master network health view: BGW, UniFi, NetFlow, DNS, and open problems |
| [firewall-dashboard/](firewall-dashboard/) | Firewall Dashboard v4 | UDM syslog ingest, DNAT hits, content filter blocks, and WAN firewall blocks |
| [att-bgw320-wan-edge/](att-bgw320-wan-edge/) | AT&T BGW320 / WAN Edge v4 | BGW broadband status, GPON optical power, firewall blocks, and WAN bytes |
| [unifi-dashboard/](unifi-dashboard/) | UniFi Dashboard v3 | Active clients, WAN status, internet disruption events, and syslog health |
| [dns-dashboard/](dns-dashboard/) | DNS v4 | BIND + dnsdist query volume, top names, health check issues, and log freshness |
| [nslb-dns-load-balancer/](nslb-dns-load-balancer/) | NSLB / DNS Load Balancer | nslb and dnsdist health-check timeouts, CPU, and log volume |
| [bindplane-otel-ingest-health/](bindplane-otel-ingest-health/) | Bindplane / OTel Ingest Health | OTel collector log volume, errors, OTLP ingest lines, and edge host coverage |
| [haproxy-ingest-health/](haproxy-ingest-health/) | HAProxy Ingest Health (utility29) | HAProxy OTLP front-end log volume, freshness, and backend keyword activity |
| [proxmox-cluster/](proxmox-cluster/) | Proxmox Cluster | Proxmox VE pveproxy logs, API extension health, freshness, and CPU by node |
| [ansible-control-plane/](ansible-control-plane/) | Ansible Control Plane | Playbook run logs, error/failure rates, Git activity, and log freshness |
| [mail-server/](mail-server/) | Mail Server | Per-user mailbox stats, host resources (CPU/memory/disk), and failed logins |
| [website-stats/](website-stats/) | Website Stats | Raw web server log records |

### Home Automation

| Folder | Dashboard | What it shows |
|--------|-----------|---------------|
| [home-ops-master-landing/](home-ops-master-landing/) | Home Ops Master Landing v12 | Master ops view across the full home stack: ingest freshness, host counts, open problems |
| [home-automation-stack/](home-automation-stack/) | Home Automation Stack | Home Assistant + AppDaemon container log volume, errors, and host CPU |
| [ha-wall-kiosks/](ha-wall-kiosks/) | HA Wall Kiosks | Pi kiosk memory, swap, Wi-Fi signal, Chromium process count, and CPU |
| [home-commander/](home-commander/) | Home Commander v2 | Orchestration service request rates, API hits, HTTP 5xx errors, and CPU |

### Miscellaneous

| Folder | Dashboard | What it shows |
|--------|-----------|---------------|
| [auditlogs-time-analysis/](auditlogs-time-analysis/) | Audit Logs Time Analysis | Dynatrace audit log events over time (high-density multi-tile view) |
