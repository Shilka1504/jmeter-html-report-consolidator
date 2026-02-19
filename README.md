# JMeter HTML Report Consolidator for Azure DevOps

This repository contains an Azure DevOps pipeline that merges multiple
JMeter `.jtl` result files from different pipeline runs and generates
a single consolidated HTML report.

## Features
- Downloads JMeter artifacts from multiple pipelines
- Normalizes JTL headers
- Merges results safely
- Generates a unified JMeter HTML dashboard
- Timezone-aware report generation (Asia/Dubai)

## Use Case
Useful when JMeter tests are executed in parallel pipelines or environments
and a combined performance report is required.

## Prerequisites
- Azure DevOps Pipelines
- Apache JMeter 5.6+
- Ubuntu hosted agent

## Files
- `Combine-JMeter-Reports.yml` – Main pipeline
- `templates/download-artifact.yml` – Reusable artifact download template
