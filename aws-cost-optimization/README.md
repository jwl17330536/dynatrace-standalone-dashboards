# AWS Cost Optimization

Surfaces underutilized AWS EC2 instances and idle EBS volumes to support cost optimization decisions. Shows CPU utilization sorted from lowest to highest and EBS idle time percentages — making it easy to find candidates for rightsizing or termination.

## What it shows

- EC2 CPU utilization by instance (%)
- EC2 average CPU per instance — sorted lowest first
- EBS volume idle time (seconds/min — max 60 = 100% idle)
- EBS volume summary: idle percentage and I/O

## Pre-requisites

- **AWS integration** configured in Dynatrace (CloudWatch metrics ingestion)
- EC2 and EBS metrics flowing into Grail

## How to import

1. Open your Dynatrace tenant
2. Go to **Dashboards** → **Import**
3. Upload the `.json` file from this folder
4. The dashboard opens immediately
