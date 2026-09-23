# Mail Server

Monitors a self-hosted mail server with a mix of infrastructure metrics and mail-specific stats. Tracks per-user mailbox activity, host resources (CPU, memory, disk), network packet errors, and failed login attempts.

## What it shows

- Mailserver stats by user
- Host CPU, memory, and disk utilization
- Packet errors
- Failed server logins

## Pre-requisites

- **OneAgent** deployed on the mail server host
- Mail server logs forwarded to Dynatrace (for login failure tracking)

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
