## Prerequisites

NGINX Prometheus Exporter binary in `/usr/local/bin/nginx-prometheus-exporter` or a location of your choice.

## Installation

1. Copy `nginx_exporter.service` and `nginx_exporter.socket` to `/etc/systemd/system/`
2. Run `systemctl daemon-reload`
3. Run `systemctl start nginx_exporter`
4. Run `systemctl status nginx_exporter` to check the status of the service

## Verification

1. Run `curl http://localhost:9113/metrics` to see the metrics exposed by the exporter.