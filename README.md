# NGINX Prometheus Exporter

NGINX Prometheus exporter makes it possible to monitor NGINX or NGINX Plus using Prometheus. [repo](https://github.com/nginxinc/nginx-prometheus-exporter)

![dashboard](https://github.com/nginxinc/nginx-prometheus-exporter/blob/main/grafana/dashboard.png?raw=true)

## Running the Exporter in a Docker Compose

To start the exporter we use the `docker compose` command.

- To export NGINX metrics, run:

    ```
    cd docker
    docker compose up -d
    ```

## Verification

```
curl -s 127.0.0.1:8080/basic_status

curl http://localhost:9113/metrics
curl -u admin:password http://localhost:9113/metrics
```
