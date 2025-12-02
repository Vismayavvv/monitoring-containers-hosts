# Monitoring Stack with Prometheus, Grafana, cAdvisor, and Node Exporter
This setup allows you to monitor the resource usage of your Docker containers in real-time using Prometheus for metrics collection and cAdvisor for container statistics. You can see CPU, memory, network, and disk usage of each container and visualize it in Grafana dashboards.

# Monitoring Stack with Prometheus, Grafana, cAdvisor, and Node Exporter

This repository provides a Docker Compose setup for a full monitoring stack including:

- **Prometheus** – Monitoring and alerting toolkit.
- **Grafana** – Visualization and dashboarding tool.
- **cAdvisor** – Container resource usage monitoring.
- **Node Exporter** – Host system metrics exporter for Prometheus.

---

## Prerequisites

Before starting, ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/) (v20+ recommended)
- [Docker Compose](https://docs.docker.com/compose/install/) (v1.29+ recommended)
- Basic knowledge of environment variables and Docker

You will also need to create a `.env` file in the root directory with the following variables:

```env
PROMETHEUS_PORT=9090
GRAFANA_HTTP_PORT=3000
GRAFANA_ADMIN_USER=admin
GRAFANA_ADMIN_PASSWORD=admin
CADVISOR_PORT=8080
NODE_EXPORTER_PORT=9100
