# MiniDC Monitor

<img width="1858" height="964" alt="Screenshot from 2026-03-06 16-22-16" src="https://github.com/user-attachments/assets/846e15b3-7d3e-4cec-a1b5-5ce4ec1b8a3e" />


A full stack hardware monitoring solution built on a personal Linux machine, using Prometheus and node_exporter to collect system metrics and Grafana for real time visualization. Inspired by data center observability practices used in production cloud infrastructure.

## Stack
- node_exporter — collects hardware metrics (CPU, RAM, disk, network, temperature)
- Prometheus — stores and queries metrics
- Grafana — real time dashboard visualization

## Setup
1. Install node_exporter: sudo apt install prometheus-node-exporter
2. Install Prometheus: sudo apt install prometheus
3. Install Grafana: sudo apt install grafana
4. Start all services: sudo systemctl enable --now prometheus-node-exporter prometheus grafana-server
5. Open Grafana at http://localhost:3000
6. Add Prometheus as data source at http://localhost:9090
7. Import dashboard.json

## Author
Jacob Grey — Data Center Technician | AWS Certified Solutions Architect
