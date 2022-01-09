# pgpepg <font size="3">([PostgreSQL](https://www.postgresql.org)/[Postgres-Exporter](https://github.com/prometheus-community/postgres_exporter)/[Prometheus](https://prometheus.io)/[Grafana](https://grafana.com/oss/grafana))</font>

Try the Grafana [PostgreSQL Dashboard](https://grafana.com/grafana/dashboards/9628) with zero effort.

## Starting-Stopping Containers
To start the services open your console on this directory then type the following command
```console
$ docker-compose up -d
```
Adding the `-d` flag will run all services in the background (detached mode).
<hr>
Type the following command to stop the services

```console
$ docker-compose down -v
```
Adding the `-v` flag will remove named volumes declared in the `volumes` section of the compose file and anonymous volumes attached to containers.

## View Dashboard
Go to http://localhost:3000/dashboards on your host then login with default admin username and password wich is `admin:admin`. Click `Databases` folder then click the `PostgreSQL Database` you will be redirect to the dashboard.

## Versions
- postgres:12
- bitnami/postgres-exporter:0.10.0-debian-10-r170
- prom/prometheus:v2.32.1
- grafana/grafana-oss:8.3.3
- Grafana PostgreSQL Dashboard: Revision 7