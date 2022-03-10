# Summary
Docker compose and config files to set up a local set of containers for
Prometheus and Grafana

# Setup
* **docker-compose up --no-start**
* **docker-compose start**

# Access
* Prometheus: http://localhost:9090
* Grafana: http://localhost:3000
  * Default userid/pw: admin/admin
    * Note: Automatically prompts to change pw on initial login
* Node-Exporter: **curl http://localhost:9100/metrics**

# Notes
* Node-exporter container
  * Purpose: Generating data from the local (docker host) instance just to have something to play with.
  * See: https://prometheus.io/docs/guides/node-exporter/