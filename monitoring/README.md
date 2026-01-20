# Monitoring Directory

This directory contains monitoring and observability configurations:

## Grafana (`grafana/`)
- Dashboard configurations
- Data source definitions
- Alert rules and notifications

## Prometheus (`prometheus/`)
- Prometheus configuration
- Service discovery rules
- Recording and alerting rules

## Usage
```bash
# Access monitoring services
# Grafana: http://localhost:3000
# Prometheus: http://localhost:9090

# Import dashboards
kubectl apply -f grafana/dashboards/
```