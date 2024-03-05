# Monitoring tools

Host and Container monitoring tool using Prometheus + cAdvisor + Node Exporter + Grafana.

## Set environment variables

In `.env` file:
```
GF_SECURITY_ADMIN_PASSWORD=
```

## Server certificates

Copy certificates to `certs` folder.
```
./certs/privkey.pem
./certs/fullchain.pem
```

Or, configure for HTTP protocol in `grafana/grafana.ini` file.

## Execute

```bash
docker-compose up -d
```

Access `https://host:3000`.

## References

 - [cAdvisor](https://github.com/google/cadvisor)
 - [Node exporter](https://github.com/prometheus/node_exporter)
 - [Prometheus](https://prometheus.io/)
 - [Grafana dashboards](https://grafana.com/grafana/dashboards/)