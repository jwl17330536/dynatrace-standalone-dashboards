# HA Wall Kiosks

Monitors Raspberry Pi-based wall kiosk devices running Chromium in kiosk mode. Tracks resource usage (memory, swap, Wi-Fi signal, CPU), Chromium process health, and automation remediation events — useful for detecting kiosks that need a reboot or signal boost.

## What it shows

- Memory and swap usage percentage
- Wi-Fi signal strength (dBm)
- Chromium process count (pid_count)
- CPU usage (user percentage)
- Remediator events (JSON-only logs)

## Pre-requisites

- **Log Monitoring / Grail** enabled
- Kiosk device metrics and logs forwarded to Dynatrace (via OTLP or OneAgent)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
