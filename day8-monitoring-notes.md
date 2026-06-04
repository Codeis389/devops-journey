# Day 8 - Monitoring

## What is Monitoring?
Watching server health 24/7
- Get alerts before health 24/7
- Fix problems before they become disasters

## Tools Used

- Prometheus = collects server data
- Node Exporter = sends server stats to Prometheus
- Grafana = shows beautiful dashboards

## What is Prometheus?
Open source monitoring tool
- collects metrics from servers
- stores data over time
- Used by Netflix, Uber, GitLab

## What is Node Exporter?
Agent that runs on server
- Sends CPU, RAM, Disk, Network stats
- Prometheus collects from it

## What is Grafana?
Dashboard and visualization tool
- Connects to Prometheus
- Shows beautiful charts and graphs
- Used by professional worldwide

## Installation Steps
- kubectl create namspace monitoring
- kuberctl apply -f prometheus-config.yaml
- kubectl apply -f prometheus-deployment.yaml
- kubectl apply node-exporter.yaml
- kubectl apply -f node-exporter.yaml
- kubectl apply -f grafana.yaml

## Access
- minikube service grafana -n monitoring --url
- Login: admin / admin

## Connect Prometheus to Grafana
- Connections -> Data Source -> Add -> Prometheus
- Enter Prometheus URL -> Save & Test

## Import Dashboard
- Dashboards -> New -> Import
- Enter ID: 1860 (Node Exporter Full)
- Select Prometheus -> Import

## Metrics You Can Monitor
- CPU Usage
- Memory Usage
- Disk Usage
- Network Traffic
- System Load

## Rule: Always monitor production servers!
## No monitoring = flying blind
